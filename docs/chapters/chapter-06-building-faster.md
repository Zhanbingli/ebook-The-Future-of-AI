# Chapter 6: Building Faster

*Andrew Ng on AI-Accelerated Startup Development*

### The Speed Imperative

In Andrew Ng's extensive experience building startups at AI Fund—a venture studio that launches approximately one startup per month—he's discovered that execution speed is perhaps the strongest predictor of startup success. "I find that the management team's ability to execute at speed is highly correlated with its odds of success," Ng observes from his unique vantage point of not just funding but actively co-founding companies.

This insight becomes particularly crucial in the AI era, where new technologies are enabling unprecedented acceleration in development cycles while simultaneously creating competitive pressures that demand rapid execution. The companies that can harness AI to move faster while maintaining quality will have significant advantages over those that cannot.

### The Agentic AI Revolution

According to Ng, the most important trend in AI over the past year has been the rise of agentic AI—systems that can perform multi-step reasoning and iterative problem-solving rather than simply generating single responses. "About a year and a half ago when I started to go around and give talks to try to convince people that AI agents might be a thing, I did not realize that around last summer a bunch of marketers would get a hold of this term and use it as a sticker and slap it on everything in sight," he notes with characteristic humor.

The technical distinction matters enormously for practical applications. Traditional language model usage is like asking someone to write an essay "by writing from the first word to the last word all in one go without ever using backspace." Agentic workflows allow AI to first create an outline, conduct web research, write a draft, critique it, and revise—much more like how humans actually work.

"For a lot of projects AI Fund has worked on, everything from pulling out complex compliance documents to medical diagnosis to reasoning about complex legal documents, we found that these agentic workflows are really a huge difference between it working versus not working."

### The Concreteness Imperative

One of Ng's most counterintuitive insights involves the importance of concrete versus abstract ideas. While vague concepts like "using AI to optimize healthcare assets" sound impressive and receive widespread approval, they're actually implementation dead ends.

"To me a concrete idea is one that's specified in enough detail that an engineer can go and build it," Ng explains. A concrete alternative might be: "Let's write software to let hospitals let patients book MR machine slots online to optimize usage."

The difference is crucial for execution speed. Concrete ideas provide clear direction, enabling teams to build rapidly and either validate or falsify their hypotheses quickly. Vague ideas, despite sounding more profound, actually slow progress by requiring additional layers of interpretation and decision-making.

### The Gut vs. Data Paradox

Surprisingly, Ng argues that subject matter expertise and intuition often provide faster decision-making mechanisms than data-driven approaches, especially in early-stage startups. "A subject matter expert with a good gut is often a much better mechanism for making a speedy decision," he notes.

This doesn't mean abandoning data—quite the opposite. The key is using data strategically to improve intuitive decision-making over time. When AB testing or user research provides surprising results, successful teams don't just implement the winning option but analyze why their initial intuitions were wrong, thereby improving their gut instincts for future decisions.

### The AI Coding Revolution

The transformation in software development capabilities represents one of the most dramatic changes in startup building. Ng distinguishes between two types of coding work: maintaining production systems (where AI provides perhaps 30-50% productivity gains) and building quick prototypes (where AI enables 10x or greater improvements).

"When you're building standalone prototypes, there's less integration with legacy software infrastructure, legacy data needed. Also the requirements, reliability, even scalability, even security are much lower," Ng explains. This enables a fundamentally different approach to innovation: "I find increasingly startups will systematically pursue innovations by building 20 prototypes to see what works."

### The Two-Way Door Philosophy

Jeff Bezos's concept of one-way versus two-way doors—decisions that are difficult versus easy to reverse—is being transformed by AI's impact on development speed. Traditionally, choices about software architecture, database schemas, and technical stacks were one-way doors due to the high cost of changing them.

"Choosing the software architecture of your tech stack used to be a one-way door," Ng observes. "I find that my team will more often build on a certain tech stack, a week later change your mind, let's throw the codebase away and redo it from scratch on a new tech stack."

This shift enables more experimentation and reduces the penalty for early technical decisions, allowing teams to optimize for learning speed rather than premature optimization.

### The Democratization of Coding

Contrary to predictions that AI would eliminate the need to learn programming, Ng argues passionately for the opposite: "I think actually it's time for everyone of every job role to learn to code." He practices what he preaches—his CFO, head of talent, recruiters, and front desk personnel all know how to code.

The reasoning is practical: as coding becomes easier through AI assistance, more people should do it, not fewer. "When many decades ago the world moved from punch cards to keyboard and terminal, that made coding easier... programming languages made it easier to code and more people learned to code."

### The Product Management Bottleneck

An unexpected consequence of accelerated software development is that product management—deciding what to build and gathering user feedback—has become the primary bottleneck for many teams. "I'm seeing very interesting dynamics... a lot more of my teams have started to complain that their bottleneck is on product engineering and design because the engineers have gotten so much faster."

This has led to some teams proposing unprecedented staffing ratios, including one team that suggested having twice as many product managers as engineers—a complete inversion of traditional tech team structures.

### The Feedback Portfolio

To address the product management bottleneck, Ng advocates for a portfolio of feedback-gathering tactics ranging from fastest/least accurate to slowest/most accurate:

1. **Personal gut instinct** (fastest, surprisingly accurate for domain experts)
2. **Three friends/teammates** (quick validation)
3. **Three to ten strangers** (broader perspective)
4. **Coffee shop/hotel lobby testing** (accessible user research)
5. **100+ user prototypes** (more systematic feedback)
6. **A/B testing** (rigorous but slow)

The key insight is using data from slower methods to improve the accuracy of faster methods, creating a flywheel where teams can make increasingly good decisions more quickly.

### Understanding AI as Competitive Advantage

Ng argues that deep understanding of AI capabilities and limitations provides significant competitive advantages, particularly because this knowledge isn't yet widely distributed. "Teams that actually get it, that understand AI, do have an advantage over teams that don't, whereas if you have an HR problem, you can find someone that knows how to do it well probably."

This advantage manifests in crucial technical decisions: "If you make the right technical decision, you can solve the problem in a couple days. If you make the wrong technical decision, you could chase a blind alley for three months."

### The Building Blocks Approach

Ng's framework for understanding AI tools involves thinking of them as building blocks that can be combined in increasingly sophisticated ways. "If you own one building block... you can build some cool stuff. But if you get a second building block... you can build something more interesting."

The combinatorial explosion of possibilities as you master more building blocks—prompting, workflows, evaluations, guardrails, retrieval-augmented generation, voice interfaces, fine-tuning—creates exponentially expanding opportunity spaces for innovation.

### Practical AI Implementation

For teams implementing AI systems, Ng emphasizes several practical considerations:

**Start with Concrete Use Cases**: Rather than trying to solve broad problems, focus on specific, measurable applications where success and failure are clearly defined.

**Build Evaluation Systems**: Develop systematic ways to measure AI performance on your specific tasks, enabling rapid iteration and model comparison.

**Design for Flexibility**: Architect systems to make switching between different AI providers relatively easy, since the landscape continues evolving rapidly.

**Focus on User Value**: Remember that AI is a tool for delivering user value, not an end in itself. The most successful applications solve real problems regardless of their technical sophistication.

### The Hype Reality Check

Despite his deep involvement in AI, Ng maintains a balanced perspective on common hype narratives. He's particularly critical of claims about AI safety risks that seem designed more for promotional purposes than genuine safety concerns.

"A lot of this... AI needs so much electricity, only nuclear power is good enough... that wind solar stuff, that's just not true," he observes. "Some of these hype narratives have been amplified that I think are a distortion of what actually will be done."

### Building vs. Using Tools

When asked about the balance between building AI tools versus learning to use existing ones, Ng emphasizes that the most powerful individuals will be those who can make computers do exactly what they want. "In the future, the people that are most powerful are the people that can make computers do exactly what you want it to do."

This skill—precisely specifying desired outcomes for AI systems—will likely remain valuable regardless of how the underlying technology evolves.

### The Responsible AI Approach

Rather than focusing on abstract AI safety concerns, Ng advocates for "responsible AI"—emphasizing how people use AI tools rather than the tools themselves. "AI is neither safe nor unsafe. It is how you apply it that makes it safe or unsafe."

This perspective shifts attention from regulating technology development to ensuring appropriate application and oversight—a more practical approach for startup builders who need to focus on delivering value while being mindful of potential negative consequences.

### Advice for AI Entrepreneurs

Ng's recommendations for startup builders in the AI era emphasize both technical understanding and execution discipline:

**Master the Building Blocks**: Invest time in understanding the current generation of AI tools and how they can be combined. The landscape changes rapidly, but foundational knowledge provides lasting advantages.

**Focus on User Problems**: The most successful AI applications solve real user problems efficiently. Technical sophistication matters less than practical value delivery.

**Build and Test Rapidly**: Use AI's acceleration of prototyping to test many ideas quickly rather than betting everything on one approach.

**Stay Close to Users**: Develop systematic approaches to gathering user feedback, since product decisions increasingly determine competitive advantage.

**Prepare for Acceleration**: AI capabilities continue improving rapidly. Build applications that will become more valuable as underlying systems get better.

### The Expanding Opportunity Space

Perhaps most importantly, Ng sees the current moment as offering unprecedented opportunities for application builders. "At this moment in time, the number of opportunities, meaning the amount of stuff that is possible that no one's built yet in the world, seems much greater than the number of people with the skill to build them."

This observation suggests that execution speed and technical competence matter more than having completely unique ideas. In a world where AI capabilities are rapidly expanding and relatively accessible, the limiting factor becomes the ability to quickly identify valuable applications and execute them well.

The teams that can combine deep AI understanding with rapid execution cycles, systematic user feedback, and disciplined focus on concrete problems will be best positioned to capture the enormous opportunities emerging in this new technological landscape.

------
