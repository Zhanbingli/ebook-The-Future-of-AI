# Building AI Startups Faster: Lessons from the Trenches

**Date:** July 10, 2025  
**Source:** [YouTube Talk](https://www.youtube.com/watch?v=RNJCfif1dPY)

It's great to see all of you here today. Since this is billed as Startup School, I want to share some lessons I've learned about building startups at AI Fund. AI Fund is a venture studio where we build an average of one startup per month. Because we co-found these startups, we're deeply involved—writing code, talking to customers, designing features, and determining pricing. We've completed many iterations of not just watching others build startups, but actually being in the trenches, building startups alongside entrepreneurs.

Today, I want to share the lessons I've learned from building startups, particularly around this rapidly changing AI technology and what it enables. My focus will be on the theme of speed. For those of you looking to build a startup, I believe a strong predictor of a startup's odds of success is execution speed. I have tremendous respect for entrepreneurs and executives who can execute quickly, and new AI technology is enabling startups to move much faster than ever before.

## The AI Stack and Where Opportunities Lie

Before diving into speed, many people ask me: "Andrew, where are the opportunities for startups?" Here's how I think about the AI stack: at the lowest level are semiconductor companies, then cloud hyperscalers built on top of that, followed by AI foundation model companies. While much of the PR excitement and hype has focused on these technology layers, the biggest opportunities almost by definition must be at the application layer. We need applications to generate even more revenue so they can afford to pay the foundation, cloud, and semiconductor technology layers.

For whatever reason, media and social media don't talk about the application layer as much, but for those of you building startups, the biggest opportunities almost by definition have to be there—although opportunities certainly exist at all layers of the stack.

## The Rise of Agentic AI

One thing that's changed dramatically over the past year is what I consider the most important tech trend in AI: the rise of agentic AI. About a year and a half ago, when I started giving talks to convince people that AI agents might be significant, I didn't realize that around last summer, marketers would get hold of this term and use it as a sticker to slap on everything in sight, which somewhat diluted its meaning. But let me share why, from a technical perspective, I think agentic AI is exciting, important, and opens up many more startup opportunities.

The way most of us use large language models (LLMs) is to prompt them to generate output. We ask the AI to produce something as if we were asking a human to write an essay from the first word to the last word in one go, without ever using backspace. Humans don't do their best writing when forced to type in this linear order, and neither does AI. Despite the difficulty of this linear constraint, our LLMs perform surprisingly well.

With agentic workflows, we can ask an AI system to first write an essay outline, then conduct web research if needed, fetch relevant web pages for context, write a first draft, read and critique that draft, revise it, and so on. This creates an iterative workflow where the model thinks, researches, revises, and returns to thinking, cycling through this loop multiple times. While slower, it delivers a much better work product.

For many projects AI Fund has worked on—from parsing complex compliance documents to medical diagnosis to reasoning about complex legal documents—we've found that agentic workflows make the crucial difference between something working versus not working. Much valuable business building still involves taking existing or new workflows and implementing them as agentic workflows.

To update the AI stack picture: over the past year, a new agentic orchestration layer has emerged that helps application builders orchestrate or coordinate numerous calls to the underlying technology layers. This orchestration layer has made building applications even easier, but I believe the basic conclusion that the application layer must be the most valuable layer of the stack still holds true.

## Best Practices for Startup Speed

### Focus on Concrete Ideas

At AI Fund, we focus exclusively on concrete ideas. A concrete product idea is one specified in enough detail that an engineer can build it. For example, "let's use AI to optimize healthcare assets" is not concrete—it's too vague. Different engineers would build completely different things, and because it's not concrete, you can't build it quickly.

In contrast, "let's write software to let hospitals allow patients to book MRI machine slots online to optimize usage" is concrete. I don't know if this is a good or bad idea, but it is concrete, meaning engineers can build it quickly. If it's a good idea, you'll discover that. If it's not, you'll discover that too. Having concrete ideas buys you speed.

The deceptive thing for many entrepreneurs is that vague ideas tend to receive kudos. If you tell friends "we should use AI to optimize healthcare assets," everyone will say it's a great idea. But it's not actually a great idea in the sense of being something you can build. When you're vague, you're almost always right, but when you're concrete, you may be right or wrong. Either outcome is fine—we can discover the truth much faster, which is crucial for startups.

### The Power of Subject Matter Expertise

Finding good concrete ideas usually requires someone—perhaps you—who is a subject matter expert to think about a problem for a long time. Before starting Coursera, I spent years thinking about online education, talking to users, and developing intuitions about what would make a good edtech platform. After that long process—what YC sometimes calls "wandering the idea maze"—experts who have deeply considered a problem can make rapid decisions. When you ask such experts whether to build this feature or that feature, their gut instinct, which is instantaneous, can be a surprisingly good proxy for making quality decisions.

While I work in AI and you might think I'd emphasize data, getting data for many startups is actually a slow mechanism for making decisions. A subject matter expert with good instincts is often a much better mechanism for speedy decision-making.

### The One Hypothesis Rule

At any moment, many successful startups are pursuing one very clear hypothesis they're building out and trying to validate. Startups don't have resources to hedge and try ten things simultaneously. Pick one, pursue it doggedly, and if data tells you to lose faith in that idea, that's perfectly fine. Just pivot immediately to pursue a completely different concrete idea.

This often describes how AI Fund operates: we pursue one thing with determination until the world tells us we were wrong, then change and pursue a totally different thing with equal determination and doggedness.

If every piece of new data causes you to pivot, it probably means you're starting from too weak a knowledge base. If every customer conversation completely changes your mind, you likely don't know enough about that sector yet to have a high-quality concrete idea. Finding someone who has thought about a subject longer may put you on a better path to move faster.

## The Build-Feedback Loop Revolution

One of the biggest changes in how we build with AI involves rapidly evolving coding assistance and the build-feedback loop. When building applications, one of the biggest risks is customer acceptance—many startups struggle not because they can't build what they want, but because they build something nobody cares about.

For many application startups (less so for deep tech or technology startups), we build software (an engineering task), get feedback from users (a product management task), then based on user feedback, tweak our views on what to build and return to writing more software. We iterate around this loop many times toward product-market fit.

With AI coding assistance, rapid engineering is becoming possible in ways that simply weren't feasible before. Engineering speed is increasing rapidly while engineering costs are decreasing rapidly. This changes how we drive startups around this loop.

### The Two Types of Software Development

I categorize the software I build into two major buckets:

1. **Quick and dirty prototypes** to test ideas—build a customer service chatbot, AI to process legal documents, whatever. Build a quick prototype to see if it works.

2. **Production software**—maintaining production-ready codebases with all the complexity that entails.

When writing production-quality code, depending on which analyst report you trust (it's hard to find rigorous data), we might be 30-50% faster with AI systems. But for building quick and dirty prototypes, we're not just 50% faster—I think we're easily 10 times faster, maybe much more.

Several factors contribute to this dramatic speed increase for prototypes: there's less integration with legacy software, infrastructure, and data needed. Requirements for reliability, scalability, and even security are much lower. I know I'm not supposed to tell people to write insecure code, but I routinely tell my team: "Go ahead, write insecure code." If the software only runs on your laptop and you don't plan to maliciously hack your own laptop, insecure code is fine. Of course, once it seems to be working, make it secure before shipping it to anyone else.

I find that startups are increasingly pursuing innovation by systematically building 20 prototypes to see what works. I know there's some anxiety in AI about many proofs of concept not making it to production, but by driving the cost of proof of concepts low enough, it's actually fine if many don't see the light of day.

### The Evolution of AI Coding Tools

The AI coding assistance landscape has evolved rapidly. Three or four years ago, we had code autocomplete popularized by GitHub Copilot. Then came Cursor and Windsurf—a generation of AI-enabled IDEs that are great. Starting six or seven months ago, we began seeing a new generation of highly agentic coding assistants. I use Claude Sonnet quite a lot for coding, and Claude Code is fantastic. Since the Claude 4 release, it's become my preference, though ask me again in a few months and I may be using something different. The tools are evolving rapidly.

This new generation of highly agentic coding assistance is making developer productivity continue to grow. Being even half a generation or one generation behind makes a big difference compared to staying on top of the latest tools. My team takes really different approaches to software engineering now compared to even three or six months ago.

### Code as a Less Valuable Artifact

One surprising development: we're used to thinking of code as a valuable artifact because it was so hard to create. But because the cost of software engineering is plummeting, code is much less valuable than it used to be. I'm on teams where we've completely rebuilt a codebase three times in the past month because it's not that difficult anymore to rebuild a codebase or pick a new data schema.

You may have heard Jeff Bezos's terminology of "two-way doors" versus "one-way doors." A two-way door is a decision you can make and, if you change your mind, reverse relatively cheaply. A one-way door is a decision that's very costly or difficult to reverse. Choosing the software architecture of your tech stack used to be a one-way door. Once you built on a certain tech stack and set a database schema, it was really hard to change.

While I don't want to say it's totally a two-way door now, my team will more often build on a certain tech stack, then a week later, change our minds and throw the codebase away to redo it from scratch on a new tech stack. I don't want to overhype this—we don't do it all the time, and there are still costs to redoing work. But my team is rethinking what constitutes a one-way door versus what's now a two-way door because the cost of software engineering is much lower.

## Empowering Everyone to Build with AI

Going beyond software engineering, I believe this is a good time to empower everyone to build with AI. Over the past year, many people advised others not to learn to code on the grounds that AI would automate it away. I think we'll look back on this as some of the worst career advice ever given. As better tools make software engineering easier, more people should do it, not fewer.

When the world moved from punch cards to keyboards and terminals, it made coding easier. When we moved from assembly to high-level languages like COBOL, there were actually people arguing that now that we had COBOL, we didn't need programmers anymore. People actually wrote papers to that effect. Of course, that was wrong. Programming languages made it easier to code, and more people learned to code. Text editors, IDEs, AI coding assistants—as coding becomes easier, more people should learn to code.

I have a controversial opinion: I think it's time for everyone in every job role to learn to code. On my team, my CFO, head of talent, recruiters, and front desk person all know how to code. I see all of them performing better at their job functions because they can code. I'm probably a bit ahead of the curve—most businesses aren't there yet—but in the future, empowering everyone to code will make many people more productive.

### The Importance of Commanding Computers

When I was teaching "Generative AI for Everyone" on Coursera, we needed to generate background art using Midjourney. One of my team members knew art history, so he could prompt Midjourney with specific genres, palettes, and artistic inspirations, giving him excellent control over generated images. We used all of his generated images. In contrast, I don't know art history, so when I prompted image generation, I could write "please make pretty pictures of robots for me," but I could never achieve the control my collaborator could.

With computers, one of the most important skills of the future is the ability to tell a computer exactly what you want so it will do it for you. People with deeper understanding of computers will be able to command computers to achieve desired outcomes. Learning to code—not necessarily writing code yourself, but steering AI to code for you—seems like it will remain the best way to do that for a long time.

## The Product Management Bottleneck

With software engineering becoming much faster, I'm seeing interesting dynamics where product management work—getting user feedback and deciding what features to build—is increasingly becoming the bottleneck. Many of my teams have started complaining that they're bottlenecked on product engineering and design because the engineers have gotten so much faster.

Three to five years ago, Silicon Valley had somewhat suspicious but nonetheless typical rules of thumb: one product manager to four engineers, or one PM to seven engineers. These were standard PM-to-engineer ratios. With engineers becoming much faster while product management work isn't becoming faster at the same pace, I'm seeing this ratio shift.

Just yesterday, for the first time when planning headcount for a project, a team proposed not one PM to four engineers, but one PM to 0.5 engineers—essentially twice as many PMs as engineers. I still don't know if this is a good idea, but it's a sign of where the world is heading. I find that PMs who can code or engineers with product instincts often perform better.

## Tactics for Rapid Product Feedback

Because engineering is accelerating, having good tactics for getting rapid feedback to shape your perspective on what to build faster helps you move faster overall. Here's a portfolio of tactics for getting product feedback, ranging from faster but less accurate to slower but more accurate:

1. **Look at the product yourself and trust your gut** (fastest) - If you're a subject matter expert, this is surprisingly effective.

2. **Ask three friends or teammates for feedback** - Get them to play with your product and provide input.

3. **Ask three to ten strangers for feedback** - One of the most important skills I've learned is how to sit in coffee shops or hotel lobbies (places with high foot traffic) and respectfully ask strangers for feedback on what I'm building. This used to be easier when I was less known. I've made numerous product decisions in hotel lobbies or coffee shops with collaborators.

4. **Send prototypes to 100 testers** - If you have access to a logical group of users.

5. **A/B testing** - Contrary to what many people think, A/B testing is now one of the slowest tactics in my menu because it's just slow to ship and depends on how many users you have.

The missing piece many teams overlook: when I A/B test something, I don't just use the results to pick product A or product B. My team sits down and carefully examines the data to hone our instincts and improve our ability to use the first tactic (gut decisions) to make high-quality decisions faster. We think: "I thought this product name would work better than that product name. Clearly, my mental model of users is wrong." We sit down to update our mental model using all that data to improve the quality of our instincts for making product decisions faster.

## Understanding AI Provides Competitive Advantage

I've seen that understanding AI actually makes you move faster, and here's why. With mature technologies like mobile, many people have had smartphones for a long time. We generally know what mobile apps can do, so many people, including non-technical people, have good instincts about mobile app capabilities.

Similarly, mature job roles like sales, marketing, HR, and legal are all important and difficult, but there are enough experienced practitioners whose knowledge is relatively diffused because these fields haven't changed dramatically in recent months.

But AI is an emerging technology, so knowledge of how to do AI really well is not widespread. Teams that truly understand AI have an advantage over teams that don't. While you can find someone who knows how to solve HR problems well, if you have an AI problem, knowing how to actually solve it could put you ahead of other companies.

Questions like "What accuracy can you get for a customer service chatbot?" "Should you use prompting, fine-tuning, or agentic workflows?" "How do you get voice AI to low latency?"—there are many decisions where making the right technical choice lets you solve problems in a couple of days, while making the wrong technical choice could lead you to chase blind alleys for three months.

I've been surprised that while one bit of information theoretically should at most make you twice as fast, in practice, if you flip the wrong bit, you're not twice as slow—you spend 10 times longer chasing blind alleys. This is why having the right technical judgment really makes startups move so much faster.

## The Building Blocks of AI

Another reason I find staying on top of AI helpful for startups: over the past two years, we've had numerous wonderful generative AI tools and building blocks. This partial list includes prompting workflows, evals, guardrails, RAG (Retrieval-Augmented Generation), voice AI, async programming, ETL, embeddings, fine-tuning, graph databases, and model integration. There's a long and wonderful list of building blocks that can be quickly combined to build software that no one on the planet could have built even a year ago.

This creates many new opportunities for startups to build new things. When I learned about these building blocks, I have a mental picture: if you own one building block—say you have a basic white building block and know how to prompt—you can build some amazing stuff with that one block. But if you acquire a second building block, like knowing how to build chatbots, you now have white and black Lego bricks and can build something more interesting.

Add a blue building block, and you can build something even more interesting. Get a few red building blocks, maybe a yellow one—more interesting. Get more building blocks, and very rapidly the number of things you can combine them into grows combinatorially or exponentially. Knowing all these wonderful building blocks lets you combine them in much richer combinations.

Deep Learning.AI works with leading AI companies worldwide to catalog and teach these building blocks. When I look at the Deep Learning.AI course catalog, whenever I take these courses to learn these building blocks, I feel like I'm acquiring new components that can combine to form combinatorially or exponentially more software applications that were impossible just one or two years ago.

## Conclusion: Speed as a Success Predictor

There are many things that matter for startups, not just speed. But when I examine the startups AI Fund is building, I find that the management team's ability to execute at speed is highly correlated with odds of success.

Here's what we've learned to achieve speed:

- **Work on concrete ideas** - They must be good concrete ideas, of course.
- **Execute fast with good judgment** - As an executive, I'm judged on both the speed and quality of my decisions. Both matter, but speed absolutely matters.
- **Leverage rapid engineering with AI coding assistance** - This makes you go much faster but shifts the bottleneck to getting user feedback on product decisions.
- **Maintain a portfolio of tactics for rapid feedback** - If you haven't learned to respectfully approach strangers in coffee shops for feedback, it's not easy, but it's a valuable skill for entrepreneurs.
- **Stay on top of the technology** - This knowledge buys you speed.

The future belongs to those who can make computers do exactly what they want them to do. People who know how to use AI will be much more powerful than people who don't.

---

*This article is based on Andrew Ng's talk at Startup School, covering lessons learned from building AI startups at AI Fund, with particular focus on execution speed and practical tactics for leveraging AI technology in startup development.*