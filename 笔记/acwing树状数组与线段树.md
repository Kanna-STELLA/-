#### 注意点
==1.下标要求从1开始  错了一次了
2.子节点 容易写错，u << 1 容易写成 u >> 1，要优先检查 两次
3.其次是tr[u].l 和l的混淆 一次
4.结构体要开四倍 一次
5.数据范围最大1e5，操作1e6；（极限情况要用scanf printf）一次
***

![[Pasted image 20230324144641.png]]

## 前缀和操作
![[Pasted image 20230324145255.png]]
## 修改操作

![[Pasted image 20230324145757.png]]
### X的父节点

![[Pasted image 20230324145840.png]]

[云剪贴板 - 洛谷 | 计算机科学教育新生态 (luogu.com.cn)](https://www.luogu.com.cn/paste/3m3obex1)
***



# 线段树


![[Pasted image 20230324172718.png]]

#父节点 
#### 左节点 x << 1
#### 右节点 x<<1 | 1

#### 节点
```cpp
struct Node{
    // int sum,l,r;
    int l,r;
    int sum;
}tr[4*N];
```

#### pushup，更新sum
```cpp
void pushup(int u){
    // tr[u].sum = tr[u << 1].l + tr[u << 1 | 1].r;
    tr[u].sum = tr[u << 1].sum + tr[u << 1 | 1].sum;
}
```

#### build,初始化线段树
```cpp
void build(int u,int l,int r){
    // if(l == r) tr[u] = {w[u],l,r};
    // if(l == r) tr[u] = {w[r],l,r};
    if(l == r) tr[u] = {l,r,w[r]};
    else{
        // int mid = tr[u].l + tr[u].r >> 1;
        int mid = l + r >> 1;
        //为什么是l + r >> 1,这里是要构筑tr[u]的节点，
        // 漏
        tr[u] = {l,r};
	    
        // 因为这个地方的赋值，所以前面的结构体要写成l,r,sum
        // build(u<<1,tr[u].l,mid),build(u<<1|1,mid+1,tr[u].r);
        build(u<<1,l,mid),build(u<<1|1,mid+1,r);
        pushup(u);
    }
}
```

#### query求前缀和
![[Pasted image 20230325104745.png]]

###### 找和l，r有交集的区间（区间mid在l，r内），完整区间直接返回
```cpp
int query(int u,int l,int r){
    if(tr[u].l >= l && tr[u].r <= r) return tr[u].sum;
    int mid = tr[u].l + tr[u].r >> 1;
    //为什么是tr[u].l + tr[u].r>> 1,这里是要顺着已有的tr[u]的节点往下搜寻
    int sum = 0;
    //判断哪个节点可以取
    if(l <= mid) sum += query(u << 1,l,r);
    // else sum += query(u << 1 | 1, l, r);
    if(r > mid) sum += query(u<<1|1,l,r);
    //也可以写r >= mid
    //可以写sum
    return sum;
}
```

#### modify，add元素
```cpp
void modify(int u,int x,int v){
    if(tr[u].l == tr[u].r) tr[u].sum += v;
    else{
        int mid = tr[u].l + tr[u].r >> 1;
        //为什么是tr[u].l + tr[u].r>> 1,这里是要顺着已有的tr[u]的节点往下搜寻
        // if(tr[u].l <= mid) modify(u << 1, x , v);
	        //查找x的位置，所以使用x来和mid比较 q w      
        if(x <= mid) modify(u << 1, x , v);
        else modify(u << 1 | 1 , x , v);
        pushup(u);
    }
}
```
#码
[云剪贴板 - 洛谷 | 计算机科学教育新生态 (luogu.com.cn)](https://www.luogu.com.cn/paste/frfdndgy)