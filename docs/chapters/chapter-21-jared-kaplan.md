# Anthropic Co-founder Jared Kaplan: Scaling and the Road to Human-Level AI

**Date:** July 29, 2025  
**Speaker:** Jared Kaplan, Co-founder, Anthropic  
**Source:** [YouTube](https://www.youtube.com/watch?v=p8Jx4qvDoSo)

---

Hello everyone. I'm Jared Kaplan, and I'm going to talk briefly about scaling and the road to human-level AI. Given this audience, many of these ideas are probably familiar, so I'll keep it concise before we move to a fireside chat Q&A with Diana.

I've only been working on AI for about six years. Before that, I had a long career—the vast majority of it—as a theoretical physicist working in academia. How did I transition to AI? 

To be brief: I started in physics because my mother was a science fiction writer, and I wanted to figure out if we could build a faster-than-light drive—physics seemed like the path to that answer. I was also deeply excited about understanding the universe: How do things work? What are the fundamental trends underlying everything we observe? Questions like: Is the universe deterministic? Do we have free will? These fascinated me.

Fortunately, during my physics career, I met many fascinating, brilliant people, including many of Anthropic's founders whom I now work with daily. I was genuinely interested in their work and kept track of it. As I moved between different areas of physics—from Large Hadron Collider physics to particle physics, cosmology, and string theory—I became somewhat frustrated. I felt we weren't making progress quickly enough.

Many friends told me AI was becoming significant, but I was skeptical. I thought, "AI has been around for 50 years. SVMs aren't particularly exciting"—that was about all we knew in 2005-2009 when I was in school. But I became convinced that AI might be an exciting field to work in. I was fortunate to know the right people, and the rest is history.

## The Two Phases of AI Training

Let me discuss how contemporary AI models like Claude and ChatGPT actually work, and how scaling leads to continuous improvement.

There are two fundamental phases in training these models:

**Phase 1: Pre-training**  
We train AI models to imitate human-written data—text and, with contemporary models, multimodal data—and understand the correlations underlying that data.

[*Shows retro slide from original GPT-3 playground*]

This vintage slide from the original GPT-3 shows how, as a speaker at a journal club, you're probably unlikely to say certain things—like "elephant" in that context. Pre-training teaches models which words are likely to follow others in large corpora of text and now multimodal data.

**Phase 2: Reinforcement Learning**  
[*Shows interface from early Claude development*]

This slide shows our original interface for what we called "Claude zero" or "Claude negative one" back in 2022 when we were collecting feedback data. You see the interface for conversing with very early Claude versions and selecting which response was better—according to you, crowdworkers, and others. Using that signal, we optimize and reinforce behaviors chosen as helpful, honest, and harmless, while discouraging poor behaviors.

Essentially, training these models involves two steps: learning to predict the next word, then using reinforcement learning to master useful tasks.

## The Discovery of Scaling Laws

It turns out there are scaling laws for both training phases.

[*Shows scaling law chart*]

This figure, which we created five or six years ago, demonstrates how scaling up AI's pre-training phase predictably yields better performance. This discovery emerged because I was asking the simplest possible questions—that's what physicists are trained to do. Look at the big picture and ask fundamental questions.

I'd heard that "big data" was important in the 2010s, so I simply wanted to know: How big should the data be? How important is it? How much does it help? Similarly, people noticed that larger AI models performed better, so we asked: How much better?

We got incredibly lucky. We found something very precise and surprising underlying AI training—trends as accurate as anything in physics or astronomy. This gave us tremendous conviction that AI would keep getting smarter in a predictable way.

As you can see in these figures from 2019, we were already looking across many orders of magnitude in compute, dataset size, and neural network size. When you observe something consistent across many orders of magnitude, you expect it will likely continue much further.

This has been one of the fundamental drivers of AI improvement. But there's another crucial element that appeared long ago but became highly impactful recently: scaling laws in the reinforcement learning phase of AI training.

## Scaling Laws in Reinforcement Learning

About four years ago, a researcher decided to study scaling laws for AlphaGo, combining two high-profile AI successes: GPT-3's scaling for pre-training and AlphaGo. This was researcher Andy Jones working independently with perhaps just a single GPU in those ancient days. Since he couldn't study expensive AlphaGo, he studied a simpler game called Hex.

[*Shows plot with ELO scores*]

ELO scores—chess ratings—describe how likely one player is to beat another in chess. They're now used to benchmark AI models by measuring how often humans prefer one AI model over another. Jones examined how different models performed as they trained to play Hex, a simple board game simpler than Go, and observed remarkable straight lines.

Noticing very simple trends is a crucial skill in science. I think this scaling behavior in reinforcement learning went unnoticed initially—people didn't focus on it soon enough—but eventually, it came to pass.

We can scale up compute in both pre-training and reinforcement learning to achieve better performance. This is the fundamental driver of AI progress. It's not that AI researchers suddenly became smarter—we found a systematic way to improve AI and we're turning that crank.

## Two Axes of AI Capabilities

I think of AI capabilities along two dimensions:

**Y-Axis: Flexibility of AI**  
The less interesting but important axis—AI's ability to meet us where we are. AlphaGo would sit far below the x-axis because, while superhuman at Go, it could only operate within that game's universe. Since large language models emerged, we've made steady progress creating AI that handles all the modalities humans can manage. We don't yet have AI models with smell, but that's probably coming. Moving up this axis gives us AI systems capable of increasingly relevant real-world tasks.

**X-Axis: Task Complexity**  
The more interesting dimension—how long it would take a person to complete the tasks AI models can handle. This has been steadily increasing as AI capability improves. This represents the time horizon for tasks.

An organization called Meter studied this systematically and found another scaling trend: the length of tasks AI models can perform doubles roughly every seven months. The increasing intelligence baked into AI through scaled compute for pre-training and reinforcement learning leads to predictable, useful tasks of increasing complexity and longer horizons.

## Looking Ahead: The Path to Human-Level AI

You can speculate about where this leads. As some AI researchers have suggested, over the next few years we may reach a point where AI models can handle tasks taking not just minutes or hours, but days, weeks, months, or years. Eventually, we envision AI models—or millions working together—doing the work of entire human organizations or scientific communities.

One advantage of mathematics or theoretical physics is that you can make progress through pure thinking. Imagine AI systems working together to achieve the progress that the theoretical physics community makes over 50 years, but in days or weeks.

If scaling can take us this far, what remains? I believe what may be needed for human-level AI is relatively straightforward:

**1. Relevant Organizational Knowledge**  
AI models that don't greet you with a blank slate but can work within companies, organizations, and governments as if they have the context of someone who's worked there for years. AI models need to work with accumulated knowledge.

**2. Memory**  
What is memory if not knowledge? I distinguish this as the ability to track progress on very long tasks, build relevant memories, and use them effectively. We've begun building this into Claude 4, and I think it will become increasingly important.

**3. Oversight**  
AI models' ability to understand fine-grained nuances and solve complex, ambiguous tasks. Right now, we see explosive progress training AI models for tasks with clear success metrics—writing code that passes tests or answering math questions correctly—because it's easy to apply reinforcement learning when success is crisp. But we need AI models that generate nuanced reward signals so we can use reinforcement learning for tasks like telling good jokes, writing good poems, and demonstrating good research taste.

The remaining ingredients are simpler: training AI models for increasingly complex tasks, progressing up the capability axis from text models to multimodal models to robotics. Over the next few years, I expect continued gains from scale applied to these different domains.

## Preparing for the Future: Three Recommendations

**1. Build Things That Don't Quite Work Yet**  
This is probably always good advice—we should maintain ambition. But specifically, AI models are improving rapidly, and I believe this will continue. If you build a product that doesn't quite work because Claude 4 is still somewhat limited, you can expect Claude 5 to make that product functional and valuable. Experiment at the boundaries of AI capability because those boundaries are moving rapidly.

**2. Use AI to Integrate AI**  
I think a major AI bottleneck is that it's developing so quickly we haven't had time to integrate it into products, companies, and everything else we do, including science. To accelerate this process, leveraging AI for AI integration will be extremely valuable.

**3. Find Rapid Adoption Opportunities**  
This might be obvious for this audience, but identifying where AI adoption can happen very quickly is key. We're seeing explosive AI integration in coding for many reasons—software engineering is ideal for AI—but the big question is: what's next? What beyond software engineering can grow that rapidly? I don't know the answer, but hopefully, you'll figure it out.

---

That concludes the presentation. Now I'd like to invite Diana on stage for our conversation.

---

## Fireside Chat: Key Insights

**Diana:** That was an excellent overview of scaling laws. Anthropic recently launched Claude 4. How does this change what's possible as model releases continue compounding over the next 12 months?

**Jared:** We'd be in trouble if it takes 12 months for an even better model! Regarding Claude 4: Claude 3.7 Sonnet was already exciting for coding, but everyone noticed it was sometimes overeager—it really wanted to make tests pass and would implement solutions you didn't want, like excessive try-catch blocks.

With Claude 4, we've improved the model's ability to act as an agent—specifically for coding, but also for search and many other applications. We've also improved its supervision and oversight capabilities so it follows directions better and hopefully improves code quality.

Another significant improvement is memory capability. Claude 4 can save and store memories, retrieving them to continue work across multiple context windows when handling complex, extended tasks.

The picture scaling laws paint is one of incremental progress. What you'll see with Claude is steady improvement across many dimensions with each release. Scaling suggests a smooth curve toward human-level AI or AGI.

**Diana:** Many YC companies have shifted from co-pilot products requiring human approval to end-to-end task replacement. How do you see this human-AI collaboration evolving?

**Jared:** It depends on acceptable performance levels. Some tasks only need 70-80% accuracy, while others require 99.9% reliability for deployment. Honestly, building for use cases where 70-80% suffices is probably more fun because you can work at the frontier of AI capability. But we're also improving reliability.

Right now, human-AI collaboration is most interesting because advanced tasks really need humans in the loop. Long-term, more tasks will be fully automated, but we're not there yet.

The future likely involves leveraging AI's breadth of knowledge. During pre-training, AI models absorb all of human civilization's knowledge. There's tremendous opportunity in using this feature—that AI knows much more than any individual human expert—to generate insights by combining knowledge across many different areas of expertise.

**Diana:** Are there specific areas where builders could focus that have more greenfield opportunities?

**Jared:** I come from a research rather than business background, so my insights may be limited. But generally, any area requiring significant skill involving computer-based data interaction seems promising: finance, people who use Excel extensively, and potentially law—though law may be more regulated and require human expertise as validation.

Another major opportunity is integrating AI into existing businesses. When electricity emerged, there was a long adoption cycle. The first applications weren't necessarily optimal—you didn't want to simply replace a steam engine with an electric motor; you wanted to remake how factories operated entirely. Similarly, leveraging AI to integrate AI into economic sectors as quickly as possible offers tremendous leverage.

**Diana:** How has your physics background influenced your ability to conduct world-class AI research?

**Jared:** The most valuable aspect was learning to identify the biggest, most macro trends and make them as precise as possible. I remember meeting brilliant AI researchers who would say things like "learning is converging exponentially," and I'd ask seemingly simple questions: "Are you sure it's exponential? Could it be a power law? Is it quadratic? Exactly how is this converging?"

These seem like basic questions, but there was significant opportunity in making observed trends as precise as possible. This provides powerful tools and helps you understand what it really means to move the needle.

With scaling laws, the holy grail is finding a better slope because that means as you invest more compute, you gain bigger advantages over other AI developers. Until you've made the observed trend precise, you don't know exactly what it means to beat it, by how much, or how to systematically determine if you're achieving that goal.

These were the primary tools I used. It wasn't necessarily applying quantum field theory directly to AI—that's too specific. AI is still incredibly young in its current incarnation—maybe 10-15 years old in terms of how we train models. It's a new field where many basic questions remain unanswered, particularly around interpretability and how AI models actually work. There's tremendous opportunity to learn at that fundamental level rather than applying highly sophisticated techniques.

-----
*This refined version maintains the authenticity and technical depth of the original while improving clarity, flow, and organization. The content remains faithful to Jared Kaplan's insights while incorporating relevant recent developments in AI scaling and Claude 4's capabilities.*