# Nobel Laureate John Jumper: AI is Revolutionizing Scientific Discovery

**Date:** July 15, 2025  
**Speaker:** John Jumper, Nobel Laureate, Senior Staff Research Scientist at Google DeepMind  
**Source:** [YouTube](https://www.youtube.com/watch?v=2Yguz5U-Nic)

---

This is a welcome change. I've given many scientific talks where no one claps or cheers when I enter. It's exciting and wonderful to be here.

I should begin by introducing myself, as not everyone in this hall may know who I am. I'm someone who has worked on AI for science and genuinely believes we can use these AI systems, technologies, and ideas to change the world in a very specific way—to accelerate science and enable new discoveries. We have an extraordinary opportunity to take these tools and ideas and direct them toward the fundamental question: How can we build the right AI systems so that sick people can become healthy and go home from the hospital?

This has been a wonderful and winding journey that brought me here today.

## From Physics to Biology to Machine Learning

I was originally trained as a physicist. I thought I'd become a "laws of the universe" physicist—if I was very lucky, I might contribute something worthy of one sentence in a textbook. I pursued physics and began a PhD, but what I was working on didn't capture my interest. It didn't feel like what I wanted to do, so I dropped out.

I didn't start a startup—that would have been very appropriate for this event—but I did end up working at a company doing computational biology: How do we get computers to say something intelligent about biology? I loved it, not just because it was fascinating, but because it allowed me to do what I thought I was good at: write code, manipulate equations, think deeply about the nature of the world, and apply these skills toward a practical purpose. Ultimately, we wanted to make medicines or enable others to make medicines.

I became both a biologist and a machine learner. Actually, I became a machine learner because I left that job and returned to graduate school in biophysics and chemistry. I no longer had access to the incredible computer hardware from my previous job—they had custom ASICs for simulating how proteins move. Since I didn't have that hardware anymore but still wanted to work on the same problems, I didn't want to simply do the same work with less compute.

I began learning statistics and machine learning. We didn't call it AI then—in fact, we didn't even call it machine learning, as that was somewhat disreputable. I said I was working in statistical physics. But the question remained: How are we going to develop algorithms? How can we learn from data and do that instead of relying solely on massive computation? It turns out AI requires both large computation and new approaches to solve novel problems.

After this, I joined Google DeepMind, a company determined to take these powerful technologies and emerging ideas—which were becoming very apparent in their power through applications to games, data centers, and other areas—and use them to advance science and push forward the scientific frontier. How could we do this in an industrial setting with incredible pace, brilliant people, excellent computer resources? With all that, you'd better make progress, and it's been tremendously fun.

The fact that I'm on this stage indicates we made some progress. The guiding principle for me has been that ultimately, we're building tools that enable scientists to make discoveries.

## The Impact: 35,000 Citations and Real Science

What I find truly heartening about our work—what still resonates with me at my core—is that AlphaFold has generated approximately 35,000 citations. Within those citations are tens of thousands of examples of people using our tools to conduct science I couldn't do alone, using them to make discoveries in vaccines, drug development, and understanding how the body works. That's genuinely exciting.

Today I want to tell you about the problem we tackled, how we solved it, the crucial role of research in machine learning (not just off-the-shelf machine learning), and what happens when you build something transformative—how people use it and its impact on the world.

## The World's Shortest Biology Lesson

Let me begin with the world's shortest biology lesson: The cell is complex.

If you've only studied biology in high school or college, you might imagine the cell as a few labeled parts—relatively simple. But cells actually resemble what you see on screen: dense, complex, crowded like a swimming pool on the Fourth of July, filled with enormous complexity.

Humans have approximately 20,000 different types of proteins—some of the structures you see on screen. They collaborate to perform practically every cellular function. You can see the green tail, which is the flagellum of E. coli—that's how it moves. Notice how it rotates and drives this motor. All of this is made of proteins.

When people say DNA is the instruction manual for life, this is what it's instructing you to build: tiny machines. Biology has evolved an incredible mechanism to construct the machines it needs—literal nanomachines built from atoms.

Your DNA provides instructions: build a protein. You might note that DNA is linear, and proteins are also linear in a sense—instructions for attaching one molecular building block after another, where each building block represents a specific atomic arrangement. But if your DNA is linear and you are decidedly not one-dimensional, what happens in between?

After you construct this protein and assemble it piece by piece, it spontaneously folds into a shape—like opening an IKEA bookshelf that assembles itself instead of requiring your hard work. You get this complex structure, a typical protein called kinase for the biologists in the audience. You can see this intricate atomic arrangement, and that arrangement is functional. The majority of proteins in your body undergo this transformation, and that determines function.

This is incredibly small. Light itself measures a few hundred nanometers, while proteins measure just a few nanometers—smaller than what you can observe under a microscope.

## The Protein Structure Challenge

For decades, scientists have wanted to understand protein structure because they use it to predict how changes in proteins might affect disease. How does biology work? Often, when you create a drug, it's designed to interrupt a specific protein's function.

Scientists have used tremendous cleverness to determine many protein structures, but it remains exceptionally difficult. Don't imagine this as simply opening a lab protocol for protein structure determination and following steps. It requires cleverness, ideas, and discovering multiple approaches.

I'm describing one type of experimental protein structure determination: convincing that large, complex molecule to form a regular crystal like table salt. No one has an easy recipe for this. They try many approaches, have ideas, and it's exceptionally difficult and filled with failure—like many scientific endeavors.

Here's one way to understand the difficulty. I found an ordinary paper we were using, flipped to the back, and read in their protocol: "After more than a year, crystals began to form." They not only conducted these challenging experiments but waited about a year to discover if it worked. That year probably wasn't spent waiting—it was spent trying thousands of other approaches that failed.

Once successful, you take this to a synchrotron—a modest instrument (you can see cars providing scale)—to shine incredibly bright X-rays and obtain a diffraction pattern. You solve that pattern and deposit it in the Protein Data Bank (PDB).

One factor that enabled our work was that scientists 50 years ago had the foresight to recognize these structures' importance and difficulty, deciding to collect them all in one place. There's a dataset representing essentially all academic protein structure output, available to everyone. Our work used entirely public data.

Approximately 200,000 protein structures are known, increasing regularly by about 12,000 annually. But this is much smaller than the need. Obtaining the input information—the DNA that describes a protein—is vastly easier. Billions of protein sequences are being discovered. We're learning about protein sequences approximately 3,000 times faster than protein structures.

## Our Solution: AlphaFold

That covers the scientific background. Let me discuss what we accomplished, shown in this schematic diagram.

We wanted to build an AI system—actually, we didn't care if it was an AI system. One advantage of working on AI for science is you don't care how you solve the problem. Whether it's a computer program or anything else, we wanted to get from the left side (where each letter represents a specific protein building block in order) through something in the middle (AlphaFold) to the right side.

You'll see two structures there: blue represents our prediction, green represents the experimental structure that required someone's year or two of effort. To assign economic value, that's approximately $100,000. You can see we accomplished this.

## The Three Components: Data, Compute, and Research

Let me explain how we did this. Any machine learning problem has three components: data, compute, and research. I believe we tell too many stories about the first two and insufficient stories about the third.

**Data:** We had 200,000 protein structures. Everyone has access to the same data.

**Compute:** This isn't LLM scale. Our final model used 128 TPU v3 cores (roughly equivalent to one GPU per core) for two weeks. This is within academic resource scope, but importantly, when considering necessary compute, don't focus on the final model number. The real computational cost comes from all the ideas that didn't work—everything you must try to reach success.

**Research:** This is where only about two people worked directly on the problem—it's a small group that accomplishes these machine learning breakthroughs. They're typically fewer people than you might imagine, and this is where our work was truly differentiated.

We developed new ideas about bringing machine learning to this problem. Earlier systems based largely on convolutional neural networks performed reasonably well and made progress. Replacing those with transformers yields roughly the same results. But taking transformer ideas plus extensive experimentation and many additional ideas—that's when you achieve real change.

In almost all AI systems you see today, tremendous amounts of research, ideas, and what I call mid-scale ideas are involved. It's not just about the headlines mentioning transformers, scaling, or test-time inference. These are important, but they're one ingredient among many in truly powerful systems.

## Measuring Research Value

We can actually measure our research's value. AlphaFold 2 is the famous system that represented a substantial improvement. AlphaFold 1 was the world's best, but someone at the AlQuraishi lab conducted a careful experiment: they took AlphaFold 2's architecture and trained it on just 1% of available data, demonstrating that AlphaFold 2 trained on 1% of data was as accurate or more accurate than AlphaFold 1, the previous state-of-the-art system.

This provides clear evidence that the third ingredient—research—was worth a hundredfold increase over the first ingredient—data. This is crucially important for anyone considering startups: think about how ideas, research, and discoveries amplify data and compute. They work synergistically. We wouldn't want less data or compute than available, but ideas are a core component in machine learning research that truly helps transform the world.

## The Importance of Mid-Scale Ideas

We can examine which components matter through ablation studies. Don't focus too heavily on details, but this data from our paper shows the difference compared to baseline. Each idea you might remove from our final system represents discrete, identifiable concepts, some of which became incredibly popular research areas.

When our work emerged, part of it involved equivariance, and people declared: "Equivariance is the answer! AlphaFold is an equivariant system! We must research equivariance more to create even greater systems!" I was confused because the sixth row there—"no IPA" (Invariant Point Attention)—removes all equivariance from AlphaFold and hurts performance only slightly.

On this GDT scale in the left graph, AlphaFold 2 was about 30 GDT points better than AlphaFold 1, and equivariance explains only two or three points. It's not about one idea—it's about many mid-scale ideas that combine into a transformative system.

When building these systems, it's vital to consider what we call biological relevance. We had ideas that were technically better—we improved our system 1% at a time. But what really mattered was crossing the accuracy threshold that mattered to experimental biologists who didn't care about machine learning. Reaching that threshold requires extensive work and effort, but when you do, it becomes incredibly transformative.

## Rigorous Evaluation: CASP

We measured against other systems available at the time through rigorous assessment. Protein structure prediction is ahead of LLMs and general machine learning in having blind assessment. Since 1994, every two years, everyone interested in predicting protein structures gathers to predict structures of a hundred proteins whose answers are unknown to anyone except the research group that just solved them—unpublished results.

This means you truly know what works. We achieved about one-third the error of any other group in this assessment. This matters because when working on problems where you don't know the answer, you can genuinely measure performance quality. You discover that many systems don't live up to researchers' beliefs during development.

Even with benchmarks, we all overfit our ideas to benchmarks unless we have held-out data. Real-world problems are almost always harder than training problems because you learn from substantial data and apply it to very important, singular problems. Measuring well during development and when people decide whether to use your system is crucial. External benchmarks are absolutely critical for determining what works and driving progress.

These examples show typical performance for us—blind predictions that are remarkably accurate.

## Making It Available: Open Source and Database

We decided it was crucial to make this available in two ways. First, we open-sourced the code. We actually open-sourced the code about a week before releasing a database of predictions, starting with 300,000 predictions and later expanding to 200 million—essentially every protein from organisms whose genomes have been sequenced.

This made an enormous difference. One of the most interesting sociological observations was the huge difference between releasing code that specialists could use (generating some information) and making it available globally in database form.

When you release something, you check social media daily to see what's happening. Even after the CASP assessment, I'd say structure predictors were convinced this was an enormous advance that solved the problem. But general biologists—the people we wanted to reach, who didn't care about structure prediction but cared about proteins for their experiments—weren't as certain. They said, "Maybe CASP was easy. I don't know."

Then the database launched, people became curious and explored it, and the extent to which proof was social was extraordinary. People would ask, "How did DeepMind access my unpublished structure?" That was the moment they truly believed—everyone either had a protein they hadn't solved or knew someone with an unpublished protein they could compare. That's what made the difference.

Having this database, accessibility, and ease led everyone to try it and understand how it worked. Word of mouth is how trust is built.

## User Testimonials and Real Impact

You can see some testimonials: "I wrestled for three to four months trying to accomplish this scientific task. This morning I got an AlphaFold prediction and now it's much better. I want my time back." "You really appreciate AlphaFold when you run it on a protein that for a year refused to get expressed and purified"—meaning they couldn't even obtain the material to begin experiments for a year.

These testimonials are crucial. When you build the right tool and solve the right problem, it matters and changes the lives of people doing work you wouldn't do but building upon yours. It's extraordinary to see these responses and the number of people I've spoken with.

The moment I truly knew this tool mattered: there was a special issue of *Science* on the nuclear pore complex a few months after our tool's release. The special issue focused entirely on this particular, very large system of several hundred proteins. Three of the four papers in *Science* made extensive use of AlphaFold. I counted over a hundred mentions of "AlphaFold" in *Science*, and we had nothing to do with it. We didn't know it was happening. We weren't collaborating. It was simply people conducting new science using tools we had built—that's the greatest feeling in the world.

## Emergent Capabilities and Unexpected Uses

Users do remarkable things and will use tools in ways you never imagined possible. This tweet from Yoshiaki Moriwaki appeared two days after our code became available. We had predicted individual protein structures, but we were working on building a system to predict how proteins interact. This researcher thought, "Well, I have AlphaFold. Why don't I put two proteins together and add something in between?"

You could think of this as prompt engineering for proteins. Suddenly they discovered this was the world's best protein interaction prediction system. When you train on these powerful systems, they develop additional, emergent skills provided they're properly aligned.

People began finding all sorts of problems AlphaFold could solve that we hadn't anticipated. It was fascinating to watch the scientific field react in real-time to these tools' existence, discovering their limitations and possibilities. This continues as people conduct exciting work in protein design and other areas building upon either the ideas or the systems we've created.

## A Transformative Application: Molecular Syringe

One application I found particularly important demonstrates how people have learned to use it for engineering large proteins. I want to tell this story for two reasons: it's a compelling application, and it illustrates how this transforms scientific work.

People often say science is about experiments and validation: "It's great that you have all these AlphaFold predictions. Now we just need to solve all proteins the classic way so we can determine whether your predictions are right or wrong."

They're correct about one thing—science is about experiments and conducting those experiments. But they're wrong about another aspect: science is about making hypotheses and testing them, not about determining any particular protein's structure.

In this case, the question involved this protein called the contractile injection system—a mouthful, so they call it the "molecular syringe." It attaches to cells and injects proteins into them. Scientists at the Zhang Lab at MIT asked: Can we use this protein for targeted drug delivery? Can we use it to deliver gene editors like Cas9 into cells?

They tried over a hundred methods to figure out how to modify this protein (for which they had no structure—this is a post-hoc rendering) and change what it recognizes. Originally involved in plant defense, they didn't know how to modify it.

They ran an AlphaFold prediction. You can see it on the left—I wouldn't even call it an excellent AlphaFold prediction, but almost immediately they examined it and said, "Wait. Those legs at the bottom must be how it recognizes and attaches to cells. Why don't we replace those with a designed protein?"

Almost immediately after obtaining the AlphaFold prediction, they re-engineered it to add this designed protein (shown in red) targeting a new cell type. They took this system and demonstrated they could select specific cells within a mouse and inject proteins—in this case, fluorescent proteins, which you can see by the coloration—targeting desired cells within a mouse brain.

They're using this to develop a new type of targeted drug delivery system. We see many more examples where scientists use this tool to test thousands of interactions to determine likely scenarios, including discovering a new component of how eggs and sperm unite in fertilization—many discoveries built upon this foundation.

## Accelerating Scientific Discovery

I believe our work made the entire field of structural biology—biology dealing with structures—approximately 5-10% faster. The extent to which that matters for the world is enormous, and we'll see more of these discoveries.

Ultimately, structure prediction and broader AI for science should be considered incredible capabilities for amplifying experimentalists' work. We begin with scattered observations—natural data, our equivalent of all internet text—then train a general model understanding underlying rules that can complete the remaining picture.

I believe we'll continue seeing this pattern become more general as we find appropriate foundational data sources. Another property is that you start where you have data, then discover applicable problems. We find enormous advances and capabilities for understanding cellular interactions or other downstream applications by extracting scientific content from these predictions, then adapting their rules to new purposes.

This is where we observe the foundational model aspect of AlphaFold or other specialized systems. I believe we'll start seeing this in more general systems, whether LLMs or others—finding increasing amounts of scientific knowledge within them and using them for important purposes.

## The Future of AI for Science

The most exciting question in AI for science is: How general will it become? Will we find a few specialized areas where we have transformative impact, or will we develop very broad systems? I expect it will ultimately be the latter as we continue advancing.

This represents where I believe we're headed, and it encapsulates the tremendous potential for AI to revolutionize scientific discovery across all disciplines.

---

*This refined version maintains Dr. Jumper's authentic voice and technical insights while improving clarity, organization, and flow. The content preserves his enthusiasm for AI's transformative potential in science while making the complex concepts more accessible to a broader audience.*