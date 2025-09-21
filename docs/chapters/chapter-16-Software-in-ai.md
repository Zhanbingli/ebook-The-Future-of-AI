# Andrej Karpathy: Software Is Changing (Again)

- **Date:** 2025-06-19  
- **Source:** [Youtube](https://www.youtube.com/watch?v=LCEmiRjPEtQ)

Hello everyone. I'm excited to be here today to talk about software in the era of AI. I'm told that many of you are students—bachelors, masters, PhD candidates—who are about to enter the industry. I think this is an extremely unique and interesting time to enter the industry because, fundamentally, software is changing again.

I say "again" because I actually gave this talk before, but software keeps changing, so I have plenty of material for new talks. I think it's changing quite fundamentally. Software hasn't changed much at such a fundamental level for 70 years, and then it's changed about twice quite rapidly in recent years. There's simply a huge amount of work to do—a huge amount of software to write and rewrite.

## The Map of Software

Let's examine the realm of software. This is a visualization called the "map of GitHub"—all the software that's been written. These are instructions to computers for carrying out tasks in digital space. When you zoom in, you see different types of repositories—all the code that has been written.

A few years ago, I observed that software was changing and there was a new type of software emerging. I called this **Software 2.0**. The idea was that Software 1.0 is the code you write for computers, while Software 2.0 consists of neural networks—specifically, the weights of neural networks. You're not writing this code directly; rather, you're tuning datasets and running optimizers to create the parameters of neural networks.

At the time, neural networks were seen as just another classifier, like decision trees. I think this framing was more appropriate. Now we have an equivalent of GitHub in the Software 2.0 realm—Hugging Face is essentially the GitHub of Software 2.0. There's also Model Atlas where you can visualize all this "code." The giant circle in the middle represents the parameters of Flux, the image generator. Anytime someone fine-tunes a Flux model, they create a git commit in this space and generate a different image generator.

So we have:
- **Software 1.0**: Computer code that programs computers
- **Software 2.0**: Weights that program neural networks

But here's what's changed fundamentally: neural networks became programmable with large language models. This is quite new and unique—it's a new computer. I think it's worth giving it a new designation: **Software 3.0**.

Your prompts are now programs that program the LLM, and remarkably, these prompts are written in English—a very interesting programming language indeed.

## The Three Paradigms

To summarize the differences: if you're doing sentiment classification, you can write Python code for it, train a neural network, or prompt a large language model with a short English prompt. You can program the computer differently by changing that prompt.

We have Software 1.0, Software 2.0, and now Software 3.0. You've probably seen that GitHub code isn't just code anymore—there's English interspersed with code, creating a growing category of new programming approaches.

Not only is this a new programming paradigm, it's remarkable that it's in our native language of English. When this blew my mind years ago, I tweeted about it, and it captured many people's attention. My currently pinned tweet says: "Remarkably, we're now programming computers in English."

## Tesla Autopilot: A Case Study

When I worked at Tesla on Autopilot, we were trying to get cars to drive autonomously. I showed a slide demonstrating how inputs from the car go through a software stack to produce steering and acceleration commands. I observed that there was extensive C++ code (Software 1.0) and some neural networks doing image recognition (Software 2.0).

Over time, as we improved the autopilot, the neural networks grew in capability and size. Simultaneously, we deleted C++ code and migrated functionality originally written in Software 1.0 to Software 2.0. For example, stitching information across different camera images and across time was handled by neural networks, allowing us to delete substantial amounts of code.

Software 2.0 literally ate through the software stack of the autopilot. I think we're seeing the same phenomenon again—we have new software that's eating through existing stacks.

## Three Programming Paradigms

We now have three completely different programming paradigms. If you're entering the industry, it's wise to be fluent in all three because they each have pros and cons. You need to decide: Will you train a neural network? Will you prompt an LLM? Should this be explicit code?

## LLMs as Utilities and Operating Systems

Andrew Ng said years ago that "AI is the new electricity," and I think this captures something interesting. LLMs feel like utilities now. LLM labs like OpenAI, Google, and Anthropic spend capital to train LLMs (equivalent to building power grids) and then spend operational expenses to serve intelligence over APIs. We pay per million tokens, and we have utility-like demands: low latency, high uptime, consistent quality.

Like electricity, you can switch between providers using services like OpenRouter. Since LLMs are software, they don't compete for physical space like traditional utilities.

When state-of-the-art LLMs go down, it's like an intelligence brownout—the planet gets measurably less intelligent as our reliance on these models grows.

LLMs also have properties similar to semiconductor fabs. The capital expenditure required is enormous, and there are deep technology trees and R&D secrets centralizing in LLM labs. However, since this is software, it's less defensible than hardware.

But the analogy that makes the most sense is that **LLMs are like operating systems**. They're not simple commodities like electricity—they're increasingly complex software ecosystems. The ecosystem is shaping similarly to traditional OS markets: a few closed-source providers (like Windows or macOS) and open-source alternatives (like Linux, with Llama potentially filling this role).

## LLMs as New Computers

When I realized this, I sketched it out: LLMs are like new operating systems. The LLM is the CPU equivalent, context windows are memory, and the LLM orchestrates memory and compute for problem-solving.

We can extend this analogy: just as you can download VS Code and run it on Windows, Linux, or Mac, you can take an LLM app like Cursor and run it on GPT, Claude, or Gemini—it's just a dropdown selection.

We're in a 1960s-era of computing where LLM compute is expensive, forcing centralization in the cloud. We're all thin clients interacting over networks, none of us having full utilization. Time-sharing makes sense when we're just dimensions in a batch process running in the cloud.

The personal computing revolution hasn't happened yet because it's not economical. Mac Minis work well for some LLMs because single-batch inference is memory-bound, but true personal AI computing remains unclear.

When I talk to ChatGPT directly in text, I feel like I'm talking to an operating system through a terminal—direct text access to the OS. A general GUI hasn't been invented yet, though some applications have their own interfaces.

## A Unique Characteristic: Reversed Technology Diffusion

LLMs flip the usual direction of technology adoption. Typically, with transformative technologies like electricity, cryptography, computing, flight, internet, and GPS, governments and corporations are first adopters because these technologies are new and expensive. Consumer adoption comes later.

LLMs are flipped around. While early computers were about ballistics and military applications, LLMs help with everyday tasks like cooking instructions. It's fascinating that we have a magical new computer primarily helping people with daily life rather than empowering governments with special military technologies.

Corporations and governments are actually lagging behind individual adoption of these technologies—a complete reversal of the normal pattern.

## Understanding LLM Psychology

Before programming LLMs, we need to understand what they are. I think of LLMs as "people spirits"—stochastic simulations of people. The simulator is an autoregressive transformer that processes tokens sequentially with roughly equal compute per token.

Because they're trained on human-generated text, they have emergent human-like psychology.

**Superhuman Capabilities:**
- Encyclopedic knowledge and memory
- Ability to remember vastly more than individual humans
- Like Rain Man's Dustin Hoffman character with near-perfect memory

**Cognitive Deficits:**
- Hallucinations and fabricated information
- Poor self-knowledge models
- Jagged intelligence (superhuman in some domains, making basic errors in others)
- Like insisting 9.11 > 9.9 or that "strawberry" has two Rs
- Anterograde amnesia—they don't learn and consolidate knowledge over time like humans

Context windows are working memory that you must program directly. They don't naturally get smarter by default. Think of the protagonists in "Memento" or "50 First Dates"—their weights are fixed and context windows reset each morning, making work and relationships problematic.

**Security Limitations:**
- Susceptible to prompt injection
- Can leak data
- Generally gullible

You must think of these as superhuman entities with significant cognitive deficits while being extremely useful. The challenge is programming them while working around deficits and leveraging superhuman capabilities.

## Partial Autonomy Applications

Let me discuss opportunities for using these models, starting with what I call "partial autonomy apps."

For coding, you could go directly to ChatGPT and copy-paste code and bug reports. But why go directly to the operating system? It makes more sense to have a dedicated app. Many of you use Cursor, which exemplifies early LLM applications with useful properties:

**Key Properties of LLM Apps:**
1. **Context Management**: LLMs handle extensive context management
2. **Multiple Model Orchestration**: Behind the scenes, there are embedding models for files, chat models, models applying code diffs—all orchestrated for you
3. **Application-Specific GUI**: Critical for human verification. Text is hard to read and interpret; visual diffs with red/green changes are much easier to audit
4. **Autonomy Slider**: In Cursor, you can do tab completion (mostly human control), Command+K for chunk changes, Command+L for entire files, or Command+I for full repository autonomy

Perplexity demonstrates similar features: information packaging, multiple LLM orchestration, GUI for auditing (source citations you can inspect), and autonomy levels (quick search vs. deep research with 10-minute waits).

## Human-AI Cooperation

A crucial aspect of LLM apps that doesn't get enough attention: we're now cooperating with AI systems. Usually, they do generation while we do verification. It's in our interest to make this loop as fast as possible.

**Two Ways to Optimize:**
1. **Speed Up Verification**: GUIs are extremely important because they utilize our visual processing. Reading text is effortful; looking at visual representations is a highway to your brain.

2. **Keep AI on the Leash**: People get over-excited about AI agents. A 10,000-line code diff isn't useful—I'm still the bottleneck for ensuring no bugs, correct functionality, and security.

I always work in small, incremental chunks, ensuring everything is good before proceeding. The key is making the flow fast while keeping AI controlled.

## Best Practices and Education

I've seen blog posts developing best practices for LLM work. For example, vague prompts lead to AI not doing what you want, causing verification failures and spinning. It's better to spend time being concrete in prompts, increasing successful verification probability.

In my education work with AI and LLMs, I spend considerable thought on keeping AI leashed. Going to ChatGPT and saying "teach me physics" doesn't work—the AI gets lost. I envision separate apps: one for teachers creating courses, another for delivering courses to students. Both have intermediate artifacts (courses) that are auditable and consistent, keeping AI leashed to specific syllabi and project progressions.

## The Tesla Autopilot Analogy

I'm familiar with partial autonomy from five years at Tesla. Autopilot is also a partial autonomy product with similar features: instrument panel GUI showing what neural networks see, and an autonomy slider where we gradually increased autonomous tasks.

The first time I experienced a self-driving car was in 2013 with a friend from Waymo in Palo Alto. We had a perfect 30-minute drive with zero interventions. I thought self-driving was imminent—this was incredible! But here we are, 12 years later, still working on autonomy. Even now, we haven't fully solved the problem. Waymo cars may look driverless, but there's still significant teleoperation and human involvement.

Software is tricky, just like driving. When I see claims like "2025 is the year of agents," I get concerned. I think this is the **decade** of agents, requiring careful, deliberate progress with humans in the loop.

## The Iron Man Suit Model

I love the Iron Man suit analogy. It's both an augmentation (Tony Stark drives it) and an agent (autonomous flight and operation). This autonomy slider concept—we can build augmentations or agents, and we want both.

At this stage, working with fallible LLMs, I recommend building Iron Man suits rather than Iron Man robots—partial autonomy products with custom GUIs and UI/UX designed for fast human verification loops, while maintaining the possibility of increasing automation over time.

## Everyone Is Now a Programmer

Not only do we have a new programming paradigm enabling autonomy, but it's programmed in English—our natural interface. Suddenly, everyone is a programmer because everyone speaks natural language. This is extremely bullish and completely unprecedented.

Previously, you needed 5-10 years studying to do software development. This is no longer the case.

## Vibe Coding

I tweeted about "vibe coding" years ago—a shower thought I expected would fizzle. Instead, it became a major meme with its own Wikipedia page. It struck a chord, giving a name to something everyone felt but couldn't articulate.

Tom Wolf from Hugging Face shared a beautiful video of children using AI to build applications. How can you look at this and feel bad about the future? This will be a gateway drug to software development. I'm not a doomer about the future—I think it's great.

I tried vibe coding myself. I built an iOS app despite not knowing Swift, completing a basic app in one day that ran on my phone. I didn't need to spend days learning Swift first.

I also vibe-coded "Menu Genen" (menu.app), solving my problem of not understanding restaurant menu items by generating pictures of dishes. Everyone gets $5 in credits when signing up, making this a major cost center in my life—a negative revenue app!

The fascinating thing about Menu Genen was that coding was actually the easy part. Making it real—authentication, payments, domain names, deployment—was extremely slow, taking a week of browser clicking and DevOps work.

## Building for Agents

This brings me to the final part: can we build for agents so they can do this work?

We now have a new category of digital information consumers and manipulators. Previously, we had humans through GUIs and computers through APIs. Now we have agents—computers that are human-like, "people spirits on the internet" needing to interact with our software infrastructure.

**Examples of Building for Agents:**

**LLM.txt files**: Like robots.txt for web crawlers, these simple markdown files tell LLMs what domains are about. Much better than having LLMs parse HTML, which is error-prone.

**Documentation for LLMs**: Many services are transitioning documentation specifically for LLMs. Vercel and Stripe offer documentation in markdown—much easier for LLMs to understand than human-formatted docs with lists, bold text, and images.

**API-First Documentation**: Instead of "click here" instructions, provide equivalent curl commands that LLM agents can execute.

**Model Context Protocol**: Anthropic's protocol for speaking directly to agents as new consumers of digital information.

**URL Transformation Tools**: Tools like GitIngest (change github.com to gitingest.com) concatenate repository files into LLM-readable formats. DevDocs creates analyzed documentation pages for repositories.

## The Future of Software Development

While LLMs can and will be able to click around interfaces, I think it's worth meeting them halfway. Making information accessible to LLMs is less expensive and more reliable than having them navigate human interfaces.

What an amazing time to enter the industry! We need to rewrite enormous amounts of code. LLMs are like utilities and fabs, but especially like operating systems—though we're in the 1960s era of this technology.

These LLMs are fallible "people spirits" we must learn to work with. We need to adjust our infrastructure accordingly. When building LLM apps, focus on fast human verification loops and creating partial autonomy products. There's also substantial work needed in building directly for agents.

Going back to the Iron Man suit analogy, over the next decade, we'll slide the autonomy slider from left to right. It will be very interesting to see what that looks like, and I can't wait to build it with all of you.