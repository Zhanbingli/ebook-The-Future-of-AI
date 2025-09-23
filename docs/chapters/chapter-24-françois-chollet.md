# François Chollet: How We Get To AGI

*Date: July 3, 2025*  
*Source: [Youtube](https://www.youtube.com/watch?v=5QcCeSsNRks)*

---

Hi everyone, I'm François. I'm super excited to share with you some of my ideas about AGI and how we're going to get there.

## The Compute Revolution and Its Limits

This chart right here represents one of the most important facts about our world: the cost of compute has been consistently falling by two orders of magnitude every decade since 1940. There's no sign that this trend is stopping anytime soon. In AI, compute and data have long been the primary bottlenecks to what we could achieve.

In the 2010s, as you all know, with the abundance of GPU-based compute and large datasets, deep learning really started to work. Suddenly, we began making fast progress on problems that had long seemed intractable across computer vision and natural language processing. In particular, self-supervised text modeling started to work, and the dominant paradigm of AI became scaling up LLM training.

This approach was crushing almost all benchmarks. Remarkably, it was getting predictably better benchmark results as we scaled up model size and training data size with the exact same architecture and training process—those are the scaling laws that Jared told you about a few minutes ago. It really seemed like we had it all figured out, and many people extrapolated that more scale was all that was needed to solve everything and get to AGI.

Our field became obsessed with the idea that general intelligence would spontaneously emerge by cramming more and more data into bigger and bigger models. But there was one problem: we were confused about what these benchmarks really meant.

## The Difference Between Skills and Intelligence

There's a big difference between memorized skills—which are static and task-specific—and fluid general intelligence: the ability to understand something you've never seen before on the fly.

Back in 2019, before the rise of LLMs, I released an AI benchmark to highlight this difference. It's called the Abstraction and Reasoning Corpus, or ARC. From 2019 to now, with a model like GPT-4.5, there's been roughly a 50,000x scale-up of base models, yet we went from 0% accuracy on that benchmark to roughly 10%—which is not a lot. It's very close to zero when you consider that any one of you in this room would score well above 95%.

To crack general fluid intelligence, it turns out we needed new ideas beyond just scaling up pre-training and doing static inference. This benchmark wasn't about regurgitating memorized skills—it was really about making sense of a new problem that you've never seen before on the fly.

## The Shift to Test-Time Adaptation

But then last year, in 2024, everything changed. The AI research community started pivoting to a new and very different paradigm: test-time adaptation—creating models that could change their own state at test time to adapt to something new.

This wasn't about querying pre-loaded knowledge anymore. It was really about the ability to learn and adapt at inference time. Suddenly, we started seeing significant progress on ARC. Finally, we had AI that was showing genuine signs of fluid intelligence.

In particular, in December last year, OpenAI previewed its o3 model. They used a version fine-tuned specifically on ARC that showed human-level performance on that benchmark for the first time. Today, in 2025, we have suddenly moved on from the pre-training scaling paradigm and we're now fully in the era of test-time adaptation.

Test-time adaptation is all about the ability of a model to modify its own behavior dynamically based on the specific data it encounters during inference. This covers techniques like test-time training, program synthesis, and chain-of-thought reasoning, where the model tries to reprogram itself for the task at hand. Today, every single AI approach that performs well on ARC is using one of these techniques.

## Fundamental Questions About Intelligence

Today I want to answer the following questions:

First, why did the pre-training scaling paradigm not get us to AGI? If you look back just two years ago, this was the standard dogma—everybody was saying this. Today, almost no one believes this anymore. So what happened?

Next, does test-time adaptation get us to AGI this time? If that's the case, maybe AGI is already here—some people believe so.

And finally, besides test-time adaptation, what else might be next for AI?

To answer these questions, we have to go back to a more fundamental question: What is intelligence? What do we mean when we say we're trying to build AGI?

## Two Views of Intelligence

If you look back over the past decades, there have been two lines of thought to define intelligence and the goals of AI.

There's the **Minsky-style view**: AI is about making machines capable of performing tasks that would normally be done by humans. This echoes very closely the current mainstream corporate view that AGI would be a model that could perform most economically valuable tasks—80% is often quoted as the number.

But then there's the **McCarthy view**: AI is about getting machines to handle problems they have not been prepared for. It's about getting AI to deal with something new.

My view is more like the McCarthy view. **Intelligence is a process, and skill is the output of that process.** Skill itself is not intelligence, and displaying skill at any number of tasks does not show intelligence.

This is like the difference between a road network and a road-building company. If you have a road network, you can go from A to B for a specific, predefined set of A's and B's. But if you have a road-building company, you can start connecting new A's and new B's on the fly as your needs evolve.

Intelligence is the ability to deal with new situations. It's the ability to blaze fresh trails and build new roads. Attributing intelligence to crystallized behavior programs—skill programs—is a category error. You're confusing the process with its output. Don't confuse the road with the process that created the road.

## Formalizing Intelligence

To formalize this, I see intelligence as the conversion ratio between the information you have—mostly your past experience, but also any developer-imparted priors the system might have—and your operational area over the space of potential future situations that you might encounter, featuring high novelty and uncertainty.

Intelligence is the efficiency with which you operationalize past information to deal with the future. It's an efficiency ratio, and that's why using exam-like benchmarks for models is a bad idea. They're not going to tell you how close we are to AGI because human exams weren't designed to measure intelligence—they were designed to measure task-specific skill and knowledge. They were designed according to assumptions sensible for humans but not for machines, like the assumption that you haven't read and memorized all the exam questions and answers beforehand.

## Key Concepts for Measuring Intelligence

If you want to properly define and measure intelligence, here are some key concepts to take into account:

**First, the distinction between static skills and fluid intelligence**—between having access to a collection of static programs to solve known problems versus being able to synthesize brand-new programs on the fly to face problems you've never seen before. Of course, it's not binary; there's a spectrum between the two.

**Second, operational area for a given skill**—there's a big difference between being skilled only in situations very close to what you've seen before and being skilled across any situation within a very broad scope. For instance, if you know how to drive, you should be able to drive in any city, not just in a specific geofenced area. You can learn to drive in San Jose, move to Sacramento, and still drive. Again, there's a spectrum there; it's not binary.

**Lastly, information efficiency for a given skill**—how much information, data, and practice did you need to acquire that skill? Higher information efficiency means higher intelligence.

## The Shortcut Rule

The reason these definitions matter is that as engineers, we can only build what we measure. The way we define and measure intelligence isn't a technical detail—it reflects our understanding of cognition. It scopes out the questions we'll ask and determines the answers we'll get. It's the feedback signal that drives us toward our goals.

A phenomenon you see constantly in engineering is the **shortcut rule**: when you focus on achieving a single measure of success, you may succeed, but you'll do so at the expense of everything else not captured by your measure. You hit the target but miss the point.

We see this all the time on Kaggle, for instance. We saw it with the Netflix Prize, where the winning system was extremely accurate but too complex to ever be used in production—it ended up never being used, making it effectively pointless.

We also saw it in AI with chess playing. The reason the AI community set out to create programs that could play chess back in the '70s was because people expected this would teach us about human intelligence. A couple of decades later, we achieved the goal when Deep Blue beat Kasparov, the world champion. In the process, we had learned nothing about intelligence. You hit the target but miss the point.

For decades, AI has chased task-specific skill because that was our definition of intelligence. But this definition only leads to automation—exactly the kind of system we have today. We actually want AI capable of autonomous invention. We don't want to stop at automating known tasks; we want AI that could tackle humanity's most difficult challenges and accelerate scientific progress. That's what AGI is meant to be.

To achieve that, we need a new target. We need to stop targeting skills and start targeting fluid intelligence itself—the ability to adapt and invent.

## Two Definitions of AGI

One definition of AGI only encompasses automation, increasing economic productivity. Obviously, this is extremely valuable. Maybe it also increases unemployment. But the other definition unlocks invention and accelerates the timeline of science. It's by measuring what you really care about that we'll be able to make progress. We need a better target, a better feedback signal.

## The ARC Benchmark

What does that look like? My first attempt at creating a way to measure intelligence in AI systems was the ARC benchmark. I released ARC-1 back in 2019. It's like an IQ test for machines—and also humans.

ARC-1 contains 1,000 tasks like this one here. Each task is unique, meaning you cannot cram for ARC. You have to figure out each task on the fly using your general intelligence rather than memorized knowledge.

Of course, solving any problem always requires some knowledge. In most benchmarks, the knowledge priors you need are typically left implicit. In ARC, we made them explicit. All ARC tasks are built entirely on top of core knowledge priors—things like objectness, elementary physics, basic geometry, topology, and counting. These are concepts any four-year-old child has already mastered.

Solving ARC requires very little knowledge, and it's knowledge that's very much not specialized. You don't need to prepare for ARC to solve it. What makes ARC unique is that you cannot solve it purely by memorizing patterns—it really requires you to demonstrate fluid intelligence.

Meanwhile, pretty much every other benchmark out there targets fixed, known tasks that can be solved or hacked via memorization alone. That's what makes ARC fairly easy for humans but very challenging for AI. When you see a problem where a human child can perform really well but the most advanced, sophisticated AI models struggle, that's a big red flashing light telling you we're missing something—that new ideas are needed.

## ARC's Purpose and Limitations

One thing I want you to keep in mind is that ARC is not going to tell you whether a system is already AGI or not—that's not its purpose. ARC is really a tool to direct the attention of the research community toward what we see as the most important unsolved bottlenecks on the way to AGI. ARC is not the destination, and solving ARC is not the goal. ARC is really just an arrow pointing in the right direction.

ARC has completely resisted the pre-training scaling paradigm. Even after a 50,000x scale-up of pre-trained base models, their performance on ARC stayed near zero. We can decisively conclude that fluid intelligence does not emerge from scaling up pre-training. You absolutely need test-time adaptation to demonstrate genuine fluid intelligence.

Importantly, when test-time adaptation arrived last year, ARC was really the only benchmark at the time that provided a clear signal about the profound shift that was happening. Other benchmarks were saturated, so they could not distinguish between a true IQ increase and just brute force scaling.

## The Need for ARC-2

Now you see this graph and you're probably asking: clearly at this point, ARC-1 is also saturating, so does that mean we have human-level AI now? Well, not yet.

What you see on this graph is that ARC-1 was a binary test—a minimal reproduction of fluid intelligence. It only gives you two possible modes: either you have no fluid intelligence, in which case you'll score near zero like base models, or you have non-zero fluid intelligence, in which case you'll instantly score very high like the o3 model from OpenAI. Every one of you in this room would score within noise distance of 100%.

So ARC-1 saturates way below human-level fluid intelligence. Now we need a better tool—a more sensitive tool that provides more useful bandwidth and better comparison with human intelligence. That tool is **ARC-2**, which we released in March this year.

Back in 2019, ARC-1 was meant to challenge the deep learning paradigm where models are big parametric curves used for static inference. Today, ARC-2 challenges reasoning systems—it challenges the test-time adaptation paradigm.

The benchmark format is still the same, but there's much greater focus on probing compositional generalization. The tasks are still very feasible for humans, but they're much more sophisticated. As a result, ARC-2 is not easily brute-forceable.

In practice, this means that in ARC-1, for many tasks, you could just look at it and instantly see the solution without thinking too much. With ARC-2, all tasks require some level of deliberate thinking, but they still remain very feasible for humans.

We know this because we tested 400 people firsthand in person in San Diego over several days. We're not talking about people with physics PhDs here—we recruited random folks: Uber drivers, UCSD students, unemployed people. Basically, anyone trying to make money on the side. All tasks in ARC-2 were solved by at least two of the people who saw them, and each task was seen on average by about seven people.

What this tells you is that a group of 10 random people with majority voting would score 100% on ARC-2. We know these tasks are completely doable by regular folks with no prior training.

## Current AI Performance on ARC-2

How well do AI models do? If you take base models like GPT-4.5 or Llama 4, it's simple—they get 0%. There's simply no way to do these tasks via memorization alone.

If you look at static reasoning systems—systems that use a single chain of thought they generate for the task—they don't do much better. They score on the order of 1-2%, very much within noise distance of zero.

What this tells you is that to solve ARC-2, you really need test-time adaptation. All systems that do meaningfully above zero are using test-time training, but even then, they're still far below human level.

Compared to ARC-1, ARC-2 enables much more granular evaluation of test-time adaptation systems like o3. That's where you see that o3 and other systems like it are still not yet quite human level.

In my view, as long as it's easy to come up with tasks that any one of you can do—tasks that are easy for humans but that AI cannot figure out no matter how much compute you throw at it—we don't have AGI yet. You'll know we're close to having AGI when it becomes increasingly difficult to come up with such tasks. We're clearly not there yet.

## Looking Ahead: ARC-3

To be clear, I don't think ARC-2 is the final test. We're not going to stop at ARC-2. We've started development on ARC-3, and ARC-3 is a significant departure from the input-output pair formats of ARC-1 and ARC-2.

We're assessing agency—the ability to explore, to learn interactively, to set goals, and achieve goals autonomously. Your AI is dropped into a brand-new environment where it doesn't know what the controls do, doesn't know what the goal is, doesn't know what the gameplay mechanics are. It has to figure out everything on the fly, starting with what it's even supposed to do in the game.

Every single game is entirely unique. They're all built on top of core knowledge priors only, just like in ARC-1 and ARC-2. We'll have hundreds of interactive reasoning tasks like this one.

Efficiency is central to the design of ARC-3. Models won't just be graded on whether they can solve a task, but on how efficiently they solve it. We're establishing a strict limit on the number of actions a model can take, targeting the same level of action efficiency we observe in humans.

We're going to launch this in early 2026, and next month in July, we're releasing a developer preview so you can start playing with it.

## What's Still Missing?

What's it going to take to solve ARC-2 (we're still very far from it today), then solve ARC-3 (we're even further from that), maybe in the future solve ARC-4, and eventually get to AGI? What are we still missing?

I've said that intelligence is the efficiency with which you operationalize the past to face a constantly changing future. But of course, if the future you faced had really nothing in common with the past—no common ground with anything you've seen before—you could not make sense of it no matter how intelligent you were.

But here's the thing: **nothing is ever truly novel**. The universe around you is made of many different things that are all similar to each other. One tree is similar to another tree, which is also similar to your neuron. Electromagnetism is similar to hydrodynamics, which is also similar to gravity. We are surrounded by isomorphisms.

## The Kaleidoscope Hypothesis

I call this the **kaleidoscope hypothesis**. Our experience of the world seems to feature never-ending novelty and complexity, but the number of unique atoms of meaning you need to describe it is actually very small. Everything around you is a recombination of these atoms.

Intelligence is the ability to mine your experience to identify these atoms of meaning that can be reused across many different situations and tasks. This involves identifying invariant structures—things that seem to be repeated principles. These building blocks, these atoms, are called **abstractions**.

Whenever you encounter a new situation, you're going to make sense of it by recombining on-the-fly abstractions from your collection to create a brand-new model adapted to the situation.

## Two Key Components of Intelligence

Implementing intelligence will have two key parts:

**First, abstraction acquisition**—you want to be able to efficiently extract reusable abstractions from your past experience, from a feed of data, for instance.

**Then, on-the-fly recombination**—you want to be able to efficiently select and recombine these building blocks into models that are fit for the current situation.

The emphasis on efficiency here is crucial. How intelligent you are isn't just determined by whether you can do something—it's determined by how efficiently you can acquire good abstractions from past experience and how efficiently you can recombine them to navigate novelty.

If you need hundreds of thousands of hours to acquire a simple skill, you're not very intelligent. If you need to enumerate every single move on a chessboard to find the best move, you're not very intelligent. Intelligence is not just demonstrating high skill—it's really the efficiency with which you acquire and deploy these skills. It's both data efficiency and compute efficiency.

## Why Scaling Didn't Lead to AGI

At this point, you start to see why simply making our AI models bigger and training them on more data didn't automatically lead to AGI. We were missing a couple of things.

First, these models lacked the ability to do on-the-fly recombination. At training time, they were learning a lot—they were acquiring many useful abstractions—but at test time, they were completely static. You could only use them to fetch and apply a pre-recorded template.

That's a critical problem that test-time adaptation is addressing. Test-time adaptation adds recombination capabilities to our AI, and that's actually a huge step forward that gets us much closer to AGI.

But that's not the only problem. Recombination isn't the only thing missing. The other problem is that these models are still incredibly inefficient. If you take gradient descent, for instance, it requires vast amounts of data to distill simple abstractions—many orders of magnitude more data than humans need, roughly three to four orders of magnitude more.

If you look at recombination efficiency, even the latest state-of-the-art test-time adaptation techniques still need thousands of dollars of compute to solve ARC-1 at human level. That doesn't even scale to ARC-2.

## The Missing Piece: Compositional Generalization

The fundamental issue here is that deep learning models are missing **compositional generalization**—that's the thing ARC-2 is trying to measure. The reason is that there's more than one kind of abstraction, and this is really important.

I said that intelligence is about mining abstractions from data and then recombining them. There are really two kinds of abstraction—**Type 1** and **Type 2**. They're pretty similar to each other; they mirror each other.

Both are about comparing things—comparing instances and merging individual instances into common templates by eliminating certain details about the instances. Basically, you take a bunch of things, compare them, drop the details that don't matter, and what you're left with is an abstraction.

The key difference between the two is that one operates over a continuous domain and the other operates over a discrete domain.

**Type 1, or value-centric abstraction**, is about comparing things via a continuous distance function. That's the kind of abstraction behind perception, pattern cognition, intuition, and also, of course, modern machine learning.

**Type 2, or program-centric abstraction**, is about comparing discrete programs—which is to say, graphs. Instead of trying to compute distances between them, you're looking for exact structure matching, exact isomorphisms, subgraph isomorphisms. This underlies much of human reasoning. It's also what software engineers do when they're refactoring code. If you hear a software engineer talk about abstraction, they mean this kind.

## Two Forms of Abstraction

So we have two kinds of abstraction, both driven by analogy-making—either value analogy or program analogy. All cognition arises from a combination of these two forms of abstraction. You can remember them with the left-brain versus right-brain metaphor—one half for perception and intuition, the other half for reasoning, planning, and rigor.

Transformers are great at Type 1 abstraction. They can do everything Type 1 is effective for—perception, intuition, pattern cognition all work well. In that sense, transformers are a major breakthrough in AI. But they're still not a good fit for Type 2. This is why you'll struggle to train one of these models to do very simple Type 2 things like sorting a list or adding digits provided as a sequence of tokens.

## The Role of Discrete Program Search

How are we going to get to Type 2? You have to leverage discrete program search as opposed to purely manipulating continuous interpolated spaces with gradient descent. **Search is what unlocks invention beyond just automation.**

All known AI systems today that are capable of some kind of invention, some kind of creativity, rely on discrete search. Even back in the '90s, we were using genetic algorithms to come up with new antenna designs. You can take AlphaGo with Move 37—that was discrete search. More recently, the AlphaFold system from DeepMind—all discrete search systems. Deep learning doesn't invent, but search does.

## Program Synthesis vs. Machine Learning

What's discrete program search? It's basically combinatorial search over graphs of operators taken from some language, some domain-specific language (DSL).

To better understand it, you can draw an analogy between program synthesis and the machine learning techniques you already know:

In machine learning, your model is a differentiable parametric function—it's a curve. In program synthesis, it's going to be a discrete graph—a graph of symbolic operations from some language.

In ML, your learning engine—the way you create models—is gradient descent, which is very compute-efficient. Gradient descent will let you find a model that fits the data very quickly, very efficiently.

In program synthesis, the learning engine is combinatorial search, which is extremely compute-inefficient. Obviously, in machine learning, the key obstacle you run into is data density. To fit a model, you need dense sampling of the data manifold—you need a lot of data.

Program synthesis is the exact reverse. Program synthesis is extremely data-efficient. You can fit a program using only two or three examples. But to find that program, you have to sift through a vast space of potential programs, and the size of that space grows combinatorially with problem complexity. So you run into this combinatorial explosion wall.

## Combining Type 1 and Type 2 Abstraction

I said earlier that intelligence is a combination of two forms of abstraction—Type 1 and Type 2. I really don't think you're going to go very far if you go all-in on just one of them, like all-in on Type 1 or all-in on Type 2. I think that if you want to really unlock their potential, you have to combine them together.

That's what human intelligence is really good at—that's what makes us special. We combine perception and intuition together with explicit step-by-step reasoning. We combine both forms of abstraction in all our thoughts and actions everywhere.

For instance, when you're playing chess, you're using Type 2 when you calculate—when you unfold some potential moves step-by-step in your mind. But you're not going to do this for every possible move, of course, because there are too many of them. You're only going to do it for a couple of different options—like here, you're going to look at the knight, the queen. The way you narrow down these options is via intuition, via pattern recognition on the board. You build that up very much through experience—you've mined your past experience unconsciously to extract these patterns, and that's very much Type 1.

You're using Type 1 intuition to make Type 2 calculation tractable.

## The Merger Strategy

How is the merger between Type 1 and Type 2 going to work? The key Type 2 technique is discrete search over a space of programs, and the blocker you run into is combinatorial explosion. Meanwhile, the key Type 1 technique is curve fitting and interpolation on the curve. You take a lot of data and embed it on some kind of interpolating manifold that enables fast but approximate judgment calls about the target space.

The big idea is to leverage these fast but approximate judgment calls to fight combinatorial explosion and make program search tractable.

A simple analogy to understand this would be drawing a map. You take a space of discrete objects with discrete relationships that would normally require combinatorial search—like pathfinding on a subway system, for instance—and you embed these objects into a latent space where you can use a continuous distance function to make fast but approximate guesses about these discrete relationships. This enables you to keep combinatorial explosion in check while doing search.

## The Vision: Programmer-Like AI

This is what the full picture looks like—this is the system we are currently working on. AI is going to move toward systems that are more like programmers that approach a new task by writing software for it.

When faced with a new task, your programmer-like meta-learner will synthesize on-the-fly a program or model that is adapted to the task. This program will blend deep learning sub-modules for Type 1 sub-problems like perception, for instance, and algorithmic modules for Type 2 sub-problems.

These models are going to be assembled by a discrete program search system that is guided by deep learning-based intuition about the structure of program space. This search process isn't done from scratch—it's going to leverage a global library of reusable building blocks, of abstractions.

That library is constantly evolving as it learns from incoming tasks. When a new problem appears, the system is going to search through this library for relevant building blocks. Whenever, in the course of solving a new problem, you're synthesizing a new building block, you're going to upload it back to the library—much like as a software engineer, if you develop a useful library for your own work, you're going to put it on GitHub so other people can reuse it.

## The Ultimate Goal

The ultimate goal here is to have an AI that can face a completely new situation and use its rich abstraction library to quickly assemble a working model—much like a human software engineer can quickly create a piece of software to solve a new problem by leveraging existing tools and libraries.

This AI is going to keep improving itself over time, both by expanding its library of abstractions and by refining its intuition about the structure of program space.

## Introducing Tendia

This system is what we are building at Tendia, our new research lab. We started Tendia because we believe that to dramatically accelerate scientific progress, we need AI that's capable of independent invention and discovery. We need AI that could expand the frontiers of knowledge, not just operate within them.

We really believe that a new form of AI is going to be key to this acceleration. Deep learning is great at automation—it's incredibly powerful for automation—but scientific discovery requires something more.

Our approach at Tendia is to leverage deep learning-guided program search to build this programmer-like meta-learner. To test our progress, our first milestone is going to be to solve ARC using a system that starts knowing nothing at all about ARC. Ultimately, we want to leverage our system for science to empower human researchers and help accelerate scientific discovery.

---

Thank you.