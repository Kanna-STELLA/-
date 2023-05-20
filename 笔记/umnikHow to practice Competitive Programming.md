  

CP is about solving problems fast. And as absurd as it may sound, I believe that SOLVE and FAST are very different and almost independent parts, and you need to practice them separately.

Let’s look at some contest, like a CodeForces round. For the sake of simplicity let’s assume that every problem has some _difficulty_, which is a numerical value denoting how hard it is, bigger values correspond to harder problems (it is not true, but it is an ok-ish approximation, at least if we consider subjective difficulty for a fixed person). Contests are made for a wide range of participants, and problemsetters strive to make contests interesting for a wide range of participants, which means having a _smooth difficulty gradient_. Well... as smooth as it is possible with 5-6 problems.

**Graph 1**

![](https://codeforces.com/predownloaded/03/a2/03a2b7c30cd8544baa708fbfba093472efa67910.jpeg)

On the moment of a contest you have some ability to solve problems. If we assign each problem with numeric difficulty, it is reasonable to say that your problem solving ability is also a number on the same scale. But it doesn’t mean that you can solve all the problems below your level and can’t solve anything above your level... it’s more like “probability distribution”, or maybe how much time you need to solve the problem of given difficulty:

**Graph 2**

![](https://codeforces.com/predownloaded/d2/ef/d2ef4f170eec01fe2a5704e46f2772ca7c1452f0.jpeg)

The issue is this probability distribution is something close to sigmoid: You can surely solve the problems that are much lower than your level and you solve them almost instantly after reading; on the other hand, you need too much time, maybe even infinite time, to solve problems way above your level. And that interval of difficulties which is not too easy while not too hard for you is rather small. Let’s call this interval _interesting_.

Since one contest has only a few problems and should cover a wide range of difficulties, there is usually one problem in your interesting interval, rarely there are two, sometimes there are none. These are the situations to which some participants refer to as _speedforces_: your result in the contest depends on how fast you solve easy problems. I don’t want to disappoint you, but **almost every contest is a speedforces contest** in a sense that your result is mostly determined by your speed and accuracy on _easy for you_ problems or, how I call them, _problems that you already know how to solve_. In a contest, you don’t have time to come up with something completely new and original. Yes, you need to get what is the problem about, unravel some layers of reductions and implement the solution, but in a nutshell **you know how to do every small part of the problems you will solve in the contest before the contest even starts**.

What I’m trying to convey is that in a contest your goal is to solve the problem that you already know how to solve fast. By doing X you learn how to do X, so by participating in contests you learn how to solve problems fast. But then where do you learn how to solve problems?

To learn how to solve problems you need to solve problems, solve problems that you don’t yet know how to solve, but that are possible for you to come up with, maybe using a lot of time. These are the problems from the _interesting_ interval, slightly above (or below in some cases) your current level, but not too much above because otherwise you can’t solve them yet. So we need to somehow find a lot of problems near your level, how to do that? The answer is rather simple: go to a place that has a lot of problems of various difficulties and doesn’t have a time limit. It is not a contest, it is an archive.

**Graph 3**

![](https://codeforces.com/predownloaded/75/c2/75c24f9c064e6b2a59daa59ddd44d96962e24f24.jpeg)

Just by having a lot of problems archives can almost always provide a problem of needed difficulty. And you don’t really need to do anything special to achieve that: sort the problems in the archive by difficulty and solve them. After the first period when the problems are too easy for you you will always be at a level where the next problems are the right difficulty for you because after solving a hundred problems your level will rise a bit, but so will the difficulty of the next problems.

I notice that nowadays many people start from CodeForces contests, and I think it is bad and it is the underlying reason for many frustrations. Some things that come to my mind:

-   Newbies are ok with repeating problems in contests, problemsetters shouldn’t be so worried about problems being fresh — you should solve old problems in archives, learn classic techniques there and then use them in contests, contest problems need to be fresh.
-   Where will we learn stuff if in contests there are no problems on classical techniques — again, learn the techniques themselves in archives, then you will see that there actually are problems that use classical techniques in contests, and obviously, there should be no problems that just are classical in contests.
-   It is hard to make a training regime out of contests — it is, and you shouldn’t do this, contests should be only a part of training regime.
-   Contests allow that [self-deception thing](https://codeforces.com/blog/entry/98621): you can solve a lot of problems in contests, but they are the problems you already know how to solve and that doesn’t increase your level.

The questions that I anticipate (ask your questions in the comments if needed):

Q: How long do I try to solve the problem in the archive before reading the editorial? Like, 30 minutes?  
A: You don’t read the editorial. The best option is to choose an archive that doesn’t have editorials at all, so you don’t have to fight the urge to look at the solution.

Q: Ugh, and what should I do if I can’t solve the problem?  
A: Abandon it, for now, switch to a different problem, return to it after a month or so. My usual approach was to open 10-15 problems, read them carefully, think a bit, choose the one I want to try and solve now, try for some time. If I don’t feel like I’m getting anywhere, switch to another problem.

Q: Month?!  
A: Maybe even more. You need time to acquire new skills and discover new ways to look at this problem (by solving other problems). It doesn’t make sense to return in less than a month because you will only run through the same ideas you did before.

Q: Ok, but how do I learn new techniques if I don’t read editorials? I’m not supposed to invent everything on my own, am I?  
A: Most of the time you [don’t need to learn any advanced stuff](https://codeforces.com/blog/entry/92248) to solve the problem, you can’t solve it because you are [not trying hard enough](https://codeforces.com/blog/entry/47516) or [not paying attention to details](https://codeforces.com/blog/entry/62730) or just being stupid. My experience even says that most Russian schoolchildren who do CP know too many algorithms.

Q: But there are problems that require some standard things!  
A: OK, yes. The best option, in my opinion, is to have some person around who solves the same archive and is better than you. In case you are stuck on a problem for a long time (that’s not an hour, that’s several months) you should ask them “Do I have to know some standard technique to solve this?” Pay attention: not ask how to solve, or for a hint, just a yes/no question. Most of the time the answer will be “No”. In the case of a positive answer, they will be able to send you a link to an article or what to google to learn about the technique. After that, you still will have to apply this technique to the problem, and you are more likely to actually remember how to use it and why did you need it in the first place, which tremendously increases your chances to use it successfully in the future.

Q: OK, which archive should I use?  
A: It is not that important, but you should use one and stick to it. I have used [Timus](https://timus.online/) because I’m from Ural region, there are numerous others: [UVa](https://onlinejudge.org/), [SPOJ](https://www.spoj.com/), [Codeforces archive](https://codeforces.com/problemset) (has editorials and too many problems, thus a warning) etc.

To sum it up:

In archives you learn how to solve problems, in contests you learn how to do it fast. I’m not saying that contests are not needed: speed is also very important, and it is good to keep you in competitive shape. Also participating in contests is just fun, that’s also very important.

Acknowledging this and separating learning how to solve from contests can lead to better training, I believe.

How to split the time between archives and contests? Well, contests are held in some fixed time, so when there is a contest that fits into your schedule, you shouldn’t miss it. Turn to archive when [you want to practice and solve something](https://codeforces.com/blog/entry/91114) which should be often, otherwise CP is probably not for you.
## 中文
CP是关于快速解决问题的。虽然听起来很荒谬，但我认为SOLVE和FAST是非常不同的，几乎是独立的部分，你需要分别练习它们。  
  
让我们看看一些比赛，比如CodeForces比赛。为了简单起见，我们假设每个问题都有一定的难度，这个难度是一个数值，表示它有多难，数值越大对应的问题越难（这不是真的，但这是一个不错的近似值，至少如果我们考虑一个固定的人的主观难度的话）。竞赛是为广泛的参与者而举办的，问题解决者努力使竞赛对广泛的参与者产生兴趣，这意味着有一个平滑的难度梯度。好吧......在5-6个问题的情况下，尽可能的平滑。  
  

![](https://codeforces.com/predownloaded/03/a2/03a2b7c30cd8544baa708fbfba093472efa67910.jpeg)


在比赛的时候，你有一些解决问题的能力。如果我们给每个问题赋予数字难度，可以合理地说，你的解决问题的能力也是同一尺度上的一个数字。但这并不意味着你能解决所有低于你水平的问题，而不能解决任何高于你水平的问题......这更像是 "概率分布"，或者说你需要多少时间来解决特定难度的问题：  
  

![](https://codeforces.com/predownloaded/d2/ef/d2ef4f170eec01fe2a5704e46f2772ca7c1452f0.jpeg)


  
问题是这个概率分布是接近sigmoid的东西： 你肯定能解决那些比你水平低得多的问题，而且你在阅读后几乎立刻就能解决它们；另一方面，你需要太多的时间，甚至是无限的时间来解决比你水平高的问题。==而那个对你来说不太容易而又不太难的困难区间是相当小的。让我们把这个区间称为有趣的区间。  


由于一个竞赛只有几个问题，而且应该涵盖广泛的难度，==所以在你的有趣区间内通常有一个问题，很少有两个，有时没有。==这些情况就是一些参赛者所说的速度优势：你在比赛中的结果取决于你解决简单问题的速度。我不想让你失望，但几乎每场比赛都是速度型比赛，从某种意义上说，==你的成绩主要取决于你解决对你来说很容易的问题的速度和准确性，或者我称之为你已经知道如何解决的问题。在比赛中，你没有时间想出一些全新的和原创的东西。==是的，你需要了解问题是什么，解开一些层层叠叠的问题，并实施解决方案，但总的来说，在比赛开始之前，你就知道如何做你将在比赛中解决的问题的每一个小部分。  
  
我想表达的是，在比赛中，你的目标是快速解决你已经知道如何解决的问题。通过做X，你学会了如何做X，所以通过参加比赛，你学会了如何快速解决问题。但是，那么你在哪里学习如何解决问题呢？  
  
为了学习如何解决问题，你需要解决问题，解决那些你还不知道如何解决的问题，但你有可能想出的问题，也许用了很多时间。这些问题来自有趣的区间，==略高于（或在某些情况下低于）你目前的水平，但不能高出太多，因为否则你还不能解决这些问题。==因此，我们需要以某种方式找到大量接近你水平的问题，如何做到这一点？答案很简单：去一个有很多不同难度的问题的地方，而且没有时间限制。这不是一个比赛，而是一个档案。  
  

![](https://codeforces.com/predownloaded/75/c2/75c24f9c064e6b2a59daa59ddd44d96962e24f24.jpeg)

    
只要有大量的问题，档案馆几乎都能提供所需难度的问题。要做到这一点，你不需要做什么特别的事情：把档案中的问题按难度分类，然后解决它们。在第一个阶段，问题对你来说太容易了，你会一直处于一个水平，接下来的问题对你来说是合适的难度，因为在解决了一百个问题后，你的水平会提高一些，但接下来的问题的难度也会提高。  
  
我注意到现在很多人都是从CodeForces比赛开始的，我认为这很不好，这也是很多人受挫的根本原因。我想到了一些事情：  
  
-==新手可以在比赛中重复问题，==问题解决者不应该如此担心问题的新鲜度--你应该在档案中解决老问题，在那里学习经典技术，然后在比赛中使用它们，比赛问题需要新鲜。  
如果比赛中没有经典技术的问题，我们从哪里学东西呢？还是那句话，在档案中学习技术本身，然后你会发现比赛中确实有使用经典技术的问题，显然，比赛中不应该有只是经典的问题。  
很难把比赛做成训练制度--这是，你不应该这样做，比赛应该只是训练制度的一部分。  
==比赛允许自我欺骗：你可以在比赛中解决很多问题，但它们是你已经知道如何解决的问题，这并不能提高你的水平。  ==
我预计的问题（如果需要，在评论中提出你的问题）：  
  
问：在阅读社论之前，我应该尝试在档案中解决多长时间的问题？比如，30分钟？  
答：你不读社论。最好的选择是选择一个根本没有社论的档案馆，这样你就不用抵抗看解决方案的冲动了。  
  
问：唉，如果我不能解决这个问题，我应该怎么办？  
答：放弃它，暂时，换一个问题，一个月左右后再回来。我通常的做法是打开10-15个问题，仔细阅读，稍加思考，选择我现在想尝试解决的问题，尝试一段时间。如果我觉得没有进展，就换成另一个问题。  
  
问：一个月吗！？  
答：也许更多。你需要时间来掌握新的技能，发现看待这个问题的新方法（通过解决其他问题）。在不到一个月的时间内回来是没有意义的，因为你只会把以前的想法跑一遍。  
  
问：好的，但如果我不看社论，我怎么能学到新的技术？我不应该自己发明一切，是吗？  
答：大多数时候，你不需要学习任何先进的东西来解决问题，你不能解决问题是因为你不够努力，或者不注意细节，或者只是愚蠢。我的经验甚至说，大多数做CP的俄罗斯小学生都知道太多的算法。  
  
问：但有些问题是需要一些标准的东西的！你怎么看？  
答：好的，是的。在我看来，最好的选择是身边有一些解决相同档案的人，而且比你强。如果你在一个问题上卡了很久（不是一个小时，是几个月），你应该问他们 "我必须知道一些标准的技术才能解决这个问题吗？" 注意：不是问如何解决，也不是要提示，只是一个是/否的问题。大多数时候，答案会是 "不"。如果答案是肯定的，他们将能够给你一个文章的链接，或者通过谷歌来了解该技术的内容。之后，你仍然要应用这个技术来解决问题，而你更有可能真正记住如何使用它，以及为什么你首先需要它，这极大地增加了你将来成功使用它的机会。  
  
问：好的，我应该使用哪个档案？  
答：这并不重要，但你应该使用一个并坚持下去。我使用Timus，因为我来自乌拉尔地区，也有许多其他的： UVa、SPOJ、Codeforces档案（有社论和太多的问题，因此要警告）等等。  
  
总结一下吧：  
  
在档案馆里你可以学到如何解决问题，在竞赛中你可以学到如何快速解决问题。我并不是说不需要竞赛：速度也很重要，让你保持竞争状态很好。另外，参加比赛只是一种乐趣，这也是非常重要的。  
  
我相信，承认这一点并将学习如何解题与比赛分开，可以带来更好的训练。  
  
如何分配档案和比赛的时间？嗯，比赛是在一些固定的时间举行的，所以当有一个适合你的日程安排的比赛时，你不应该错过它。当你想练习和解决一些问题时，就去看档案，这应该是经常的，否则CP可能不适合你。  
  
[Translated with DeepL](https://www.deepl.com/translator?utm_source=windows&utm_medium=app&utm_campaign=windows-share)