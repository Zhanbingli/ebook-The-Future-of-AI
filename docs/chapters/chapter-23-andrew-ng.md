# Andrew Ng: Building Faster with AI

It's great to see all of you here today. Since this is Y Combinator's AI Startup School, I want to share lessons I've learned about building startups at AI Fund. AI Fund is a venture studio where we build an average of one startup per month. As co-founders of these startups, we're deeply involved—writing code, talking to customers, designing features, and determining pricing. We've done many iterations of not just watching others build startups, but actually being in the weeds, building them with entrepreneurs.

Today I want to share lessons I've learned about building startups, particularly around how this changing AI technology is enabling new possibilities. My focus will be on execution speed—which I believe is a strong predictor of startup success. I have tremendous respect for entrepreneurs and executives who can simply execute quickly, and new AI technology is enabling startups to move much faster than before.

## The AI Opportunity Stack

Many people ask me: "Where are the opportunities for startups?" I think of this as the AI stack. At the lowest level are semiconductor companies, then cloud providers and hyperscalers, then AI foundation model companies. While much of the media excitement has focused on these technology layers, the biggest opportunities are almost certainly at the application layer. This is definitional—applications need to generate enough revenue to pay for the foundation models, cloud services, and semiconductor layers beneath them.

For whatever reason, media tends to focus less on the application layer, but for those building startups, this is where the largest opportunities exist—though opportunities certainly exist at every layer of the stack.

## The Rise of Agentic AI

If you ask me about the most important AI trend today, I'd say it's the rise of agentic AI. About a year and a half ago, when I started giving talks about AI agents, I didn't realize that marketers would adopt this term and apply it to everything, which diluted its meaning. But from a technical perspective, agentic AI is both exciting and important because it opens up many more startup opportunities.

Consider how most of us use large language models—we prompt them to generate output in a linear fashion, like asking someone to write an essay from the first word to the last without ever using backspace. Humans don't do their best writing this way, and neither does AI. Despite this limitation, LLMs perform surprisingly well.

With agentic workflows, we can ask an AI system to first write an essay outline, then conduct web research and gather relevant information, then write a first draft, then critique and revise that draft, and so on. This creates an iterative workflow where the model thinks, researches, revises, and thinks again. While slower, this delivers much better work product.

At AI Fund, we've worked on projects ranging from complex compliance document analysis to medical diagnosis to legal document reasoning. We've consistently found that agentic workflows make the difference between something working and not working. Much of the valuable work ahead involves taking existing or new workflows and implementing them as agentic systems.

This has led to the emergence of a new agentic orchestration layer that helps application builders coordinate multiple calls to the underlying technology stack. While this orchestration layer makes building applications easier, the fundamental conclusion remains: the application layer represents the most valuable part of the stack.

## Building Faster: Key Principles

Let me share the best practices I've learned for helping startups move faster.

### Focus on Concrete Ideas

At AI Fund, we only work on concrete ideas—product concepts specified in enough detail that an engineer can build them. For example, "let's use AI to optimize healthcare assets" is too vague. Different engineers would build completely different things, and because it's not concrete, you can't build it quickly.

In contrast, "let's write software that lets hospital patients book MRI machine slots online to optimize usage" is concrete. An engineer can build this, and whether it's a good or bad idea, you'll find out quickly. Concrete ideas enable speed.

Vague ideas tend to receive praise—if you tell friends "we should use AI to optimize healthcare assets," everyone will say it's a great idea. But it's not actually a great idea in the sense of being buildable. When you're vague, you're almost always right, but when you're concrete, you may be right or wrong—and either way, you can discover this quickly.

Finding good concrete ideas usually requires subject matter expertise—someone who has thought deeply about a problem for a long time. For instance, before starting Coursera, I spent years thinking about online education, talking to users, and developing intuitions about what would make a good EdTech platform. After this extended process of exploring what YC sometimes calls "the idea maze," experts develop intuition that enables rapid decision-making.

While I work in AI and love data, getting data is often a slow mechanism for making decisions. A subject matter expert with good intuition often provides a much faster mechanism for quality decision-making.

### Pursue One Clear Hypothesis

Successful startups typically pursue one very clear hypothesis at any given time—building it out and trying to sell its value proposition. Startups don't have resources to hedge by trying ten things simultaneously. Pick one, commit fully, and if data tells you to abandon it, pivot completely to pursue a totally different concrete idea with equal determination.

At AI Fund, we pursue one thing with complete determination until the world tells us we're wrong, then we pivot and pursue something entirely different with equal commitment. If every piece of new data causes you to pivot, you probably started from too weak a knowledge base. Finding someone who has thought more deeply about a subject may help you identify a better path forward.

### Accelerate the Build-Feedback Loop

When building applications, one of the biggest risks is customer rejection—not because we can't build what we want, but because we build something nobody cares about. For application startups especially, we build software (an engineering task), get user feedback (a product management task), then iterate based on that feedback. We go around this loop many times, iterating toward product-market fit.

AI coding assistance is dramatically changing this dynamic. The speed of engineering is increasing rapidly while the cost is decreasing rapidly. This changes how we drive startups through this iteration loop.

I categorize software development into two buckets. Sometimes we build quick and dirty prototypes to test ideas—a customer service chatbot, AI for processing legal documents, whatever. Other times we write and maintain production software with massive, production-ready codebases.

For production-quality code, we're maybe 30-50% faster with AI systems (though rigorous data is hard to find). But for building quick and dirty prototypes, we're easily 10 times faster, possibly much more. This is because standalone prototypes require less integration with legacy software and infrastructure, and have lower requirements for reliability, scalability, and security.

I routinely tell my team to write insecure code when building prototypes that will only run on their laptops. Of course, before shipping to others, make it secure and scalable—but for testing, it's fine. This enables startups to systematically pursue innovation by building 20 prototypes to see what works.

### Leverage the Latest AI Tools

The AI coding assistance landscape evolves rapidly. We've seen code autocomplete (popularized by GitHub Copilot), then AI-enabled IDEs like Cursor and Windsurf, and now highly agentic coding assistants. I currently use Claude for coding extensively, though I expect this will change within months as tools continue evolving.

Being even half a generation behind in tools makes a significant difference compared to using the latest capabilities. My team takes fundamentally different approaches to software engineering now compared to even six months ago.

One surprising change: we used to think of code as a valuable artifact because it was difficult to create. But as the cost of software engineering decreases, code becomes less valuable as an artifact. I've seen teams completely rebuild codebases three times in a month because it's no longer prohibitively difficult.

This relates to Jeff Bezos's concept of two-way doors versus one-way doors. Two-way doors are decisions you can reverse relatively cheaply if you change your mind. One-way doors are difficult or costly to reverse. Choosing software architecture used to be a one-way door, but now my team more often builds on one tech stack, then a week later throws it away and rebuilds from scratch on a different stack.

### Empower Everyone to Build with AI

This is a good time to empower everyone to build with AI. Over the past year, many people advised others not to learn coding because AI would automate it. I believe this will be seen as some of the worst career advice ever given. As better tools make software engineering easier, more people should learn to code, not fewer.

When we moved from punch cards to keyboards and terminals, coding became easier and more people learned to code. When we moved from assembly to high-level languages like COBOL, some people argued we wouldn't need programmers anymore, but this was wrong. Programming languages made coding easier and more people learned to code.

I have a controversial opinion: it's time for everyone in every job role to learn to code. On my team, my CFO, head of talent, recruiters, and front desk person all know how to code, and I see all of them performing better at their job functions because of this capability. I'm probably ahead of the curve, but I believe empowering everyone to code will make people far more productive.

### Understand That Product Management Becomes the Bottleneck

As software engineering becomes much faster, product management work—getting user feedback and deciding what features to build—increasingly becomes the bottleneck. Over the past year, many of my teams have complained that they're bottlenecked on product and design because engineers have become so much faster.

Three to five years ago, Silicon Valley had rough rules of thumb about product manager to engineer ratios—maybe one PM to four or seven engineers. With engineers becoming much faster while product management work hasn't accelerated at the same rate, I'm seeing this ratio shift dramatically. Yesterday, for the first time, one of my teams proposed having two PMs for every engineer—a complete reversal.

I'm not sure this is a good idea, but it signals where things are heading. PMs who can code, or engineers with product instincts, often perform better in this environment.

### Develop Rapid Feedback Mechanisms

Because engineering is accelerating so rapidly, having good tactics for getting rapid feedback helps shape what you should build faster. Here's a portfolio of tactics, ordered from fastest (but less accurate) to slower (but more accurate):

1. **Look at the product yourself and trust your gut** - If you're a subject matter expert, this is surprisingly effective
2. **Ask three friends or teammates for feedback** 
3. **Ask three to ten strangers for feedback** - I've learned to identify high foot-traffic locations like hotel lobbies and respectfully approach strangers
4. **Send prototypes to 100 testers**
5. **A/B test with more users**

Contrary to what many think, A/B testing is now one of the slowest tactics because it takes time to ship and gather statistically significant results.

When using any tactic beyond the first, don't just use results to pick option A or B. Sit down and analyze the data to improve your instincts and mental models, enabling higher-quality gut decisions in the future.

## Why Understanding AI Creates Competitive Advantage

Understanding AI actually makes you go faster, and here's why. With mature technologies like mobile, many people understand what mobile apps can do. With mature job roles like sales, marketing, HR, and legal, knowledge of best practices is widely distributed because these fields haven't changed dramatically.

But AI is an emerging technology. Knowledge of how to implement AI well is not widespread, giving teams that truly understand AI a significant advantage. Things like: What accuracy can you achieve with a customer service chatbot? Should you prompt engineer or fine-tune? How do you achieve low-latency voice responses?

Making the right technical decision can solve a problem in days, while the wrong decision can lead you down a blind alley for three months. While it might seem like one bit of information can only provide a 2x speed advantage, in practice, flipping the wrong bit doesn't make you twice as slow—it makes you 10 times slower as you chase dead ends.

Additionally, we now have a tremendous array of AI building blocks: prompting, workflows, evals, guardrails, RAG, voice, async programming, ETL, embeddings, fine-tuning, graph databases, and model integration capabilities. These tools enable building software that was impossible even a year ago.

I think of this like Lego blocks. With one block, you can build something interesting. With two blocks, you can build something more interesting. As you acquire more building blocks, the number of things you can build grows exponentially. Understanding these building blocks and how to combine them creates enormous opportunities.

## Conclusion

Many factors matter for startup success beyond speed, but in the startups AI Fund builds, management team execution speed strongly correlates with success odds. To achieve this speed:

- Work on concrete ideas (but make sure they're good concrete ideas)
- Execute rapid engineering with AI coding assistance
- Develop portfolio of tactics for rapid user feedback
- Stay current with AI technology capabilities

As an executive, I'm judged on both the speed and quality of my decisions. Both matter, but speed absolutely matters. The shift to AI coding assistance moves the bottleneck to product decisions and user feedback, making rapid feedback mechanisms critical.

The amount of new things possible to build far exceeds the number of people skilled enough to build them. At the application layer especially, there's significant white space for new solutions. Focus on building products that people truly want and love, then figure out the rest along the way.

Thank you very much. I'm happy to take questions.