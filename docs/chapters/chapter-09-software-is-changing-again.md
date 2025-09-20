# Chapter 9: Software is Changing (Again)

*Andrej Karpathy on the Three Paradigms of Programming*

### The Evolution of Programming Languages

Andrej Karpathy's framework for understanding software development identifies three distinct paradigms that represent fundamentally different ways of instructing computers. Software 1.0 consists of explicit code written by humans. Software 2.0 comprises neural network weights generated through training on data. Software 3.0 involves natural language prompts that program large language models.

"We have three completely different programming paradigms, and I think if you're entering the industry, it's a very good idea to be fluent in all of them," Karpathy explains. This multi-paradigm fluency becomes crucial as different approaches prove optimal for different types of problems.

### The LLM Operating System

Karpathy's most profound insight positions large language models as a new type of operating system rather than just another application or tool. "LLMs are like a new operating system," he argues, drawing parallels between LLM architecture and traditional OS components.

The context window functions as memory, the LLM itself serves as the CPU, and various capabilities (tool use, multimodality, reasoning) operate like system services. This perspective explains why we're seeing ecosystem development patterns similar to early computing: different providers competing like Windows versus Mac versus Linux, with applications being built to run on these new platforms.

### The 1960s Computing Parallel

Current LLM deployment resembles 1960s computing more than modern personal computing. Expensive compute resources are centralized in the cloud, accessed through time-sharing by multiple users who never achieve full utilization of the underlying system. "We're like in this 1960s-ish era where LLM compute is still very expensive... and that forces the LLMs to be centralized in the cloud."

This centralization creates opportunities for the eventual "personal computing revolution" in AI—when individual users can run powerful AI systems locally rather than depending on cloud services. Early experiments with models running on devices like Mac minis hint at this transition, though the timeline remains unclear.

### The Psychology of AI Systems

Understanding LLMs requires recognizing them as "people spirits"—stochastic simulations of human behavior trained on vast amounts of human-generated text. This psychological framing helps explain both their capabilities and limitations.

Like savants with perfect memory but cognitive deficits, LLMs can recall enormous amounts of information while making basic errors that no human would make. They display "jagged intelligence"—superhuman performance in some domains coupled with surprising failures in others. They also suffer from "anterograde amnesia," unable to learn and improve from individual interactions.

### The Partial Autonomy Revolution

Rather than building fully autonomous AI agents, Karpathy advocates for "partial autonomy" applications that combine AI capabilities with human oversight. Examples like Cursor for coding and Perplexity for search demonstrate this pattern: AI handles complex processing while humans provide direction and verification.

"We're now cooperating with AIs, and usually they are doing the generation and we as humans are doing the verification," Karpathy notes. Optimizing this cooperation loop—making generation faster and verification more efficient—becomes crucial for maximizing productivity.

### The Autonomy Slider

Successful AI applications provide users with control over the level of autonomy they grant to the system. Cursor exemplifies this with options ranging from tab completion (minimal autonomy) to entire repository modification (maximum autonomy). Users can adjust based on task complexity and their comfort level.

This graduated approach recognizes that different situations call for different levels of AI involvement. Simple, well-defined tasks can handle more autonomy, while complex or sensitive work benefits from tighter human oversight.

### The GUI Imperative

As AI systems become more capable, graphical user interfaces become increasingly important for enabling effective human oversight. "Text is very hard to read, interpret, understand... but looking at stuff is fun and it's just a highway to your brain," Karpathy observes.

Visual representations allow humans to quickly audit AI work, identify errors, and provide feedback. This explains why successful AI applications invest heavily in interface design that makes AI outputs easy to understand and interact with.

### The Vibe Coding Phenomenon

Karpathy coined the term "vibe coding" to describe programming by natural language description rather than explicit syntax. This approach enables people without formal programming training to create functional software by describing what they want in English.

However, vibe coding works best for custom, one-off applications rather than production systems. The real bottleneck often lies not in writing code but in deployment, authentication, payments, and other infrastructure concerns that require more traditional software engineering.

### Building for Agents

As AI agents become more capable, software infrastructure must adapt to serve these new types of users. Just as websites include robots.txt files to instruct web crawlers, future sites may include llm.txt files to communicate directly with AI systems.

This evolution requires rethinking documentation, APIs, and user interfaces to be accessible to both humans and AI agents. Simple changes like providing markdown versions of documentation or replacing "click here" instructions with equivalent API calls can dramatically improve AI accessibility.

### The Iron Man Suit Philosophy

Karpathy's vision for AI applications draws inspiration from the Iron Man suit—technology that can function both as an augmentation tool under human control and as an autonomous agent when appropriate. This duality provides the flexibility needed for different situations and user preferences.

"It's less Iron Man robots and more Iron Man suits that you want to build," he suggests, emphasizing augmentation over replacement as the near-term opportunity for AI applications.

### Preparing for Transformation

As AI capabilities continue advancing, Karpathy sees a fundamental transformation in software development approaching. Applications will become more autonomous, interfaces will adapt to serve both human and AI users, and the distinction between human and machine-generated code will blur.

This transformation requires infrastructure investment, new design paradigms, and careful attention to the human-AI interaction model. The companies that prepare for this shift by building flexible, AI-compatible systems will be best positioned to thrive in the transformed landscape ahead.

### The Speed of Change

Perhaps most importantly, Karpathy emphasizes that this transformation is happening rapidly. "Software is changing again," he notes, and the pace of change continues accelerating. Organizations and individuals that can adapt quickly to new paradigms will have significant advantages over those that cannot.

The key is maintaining flexibility while building for the future—creating systems that work well today while preparing for the more autonomous, AI-integrated world that's rapidly approaching.

------
