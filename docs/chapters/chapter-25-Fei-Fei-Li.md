# Fei-Fei Li: Spatial Intelligence is the Next Frontier in AI

*Date: July 1, 2025*  
*Source: [Youtube](https://www.youtube.com/watch?v=_PioN-CpOP0)*

---

**Introduction**

My entire career has been about going after problems that are just so hard they're bordering on delusional. To me, AGI will not be complete without spatial intelligence, and I want to solve that problem. I just love being an entrepreneur. Forget about what you have done in the past. Forget about what others think of you. Just hunker down and build. That is my comfort zone.

I'm super excited to be here with Dr. Fei-Fei Li. She has such a distinguished career in AI—I'm sure many of you know her work. She's been named the godmother of AI. One of her first groundbreaking projects was ImageNet in 2009, 16 years ago. That project has over 80,000 citations and really kicked off one of the foundational pillars of AI: solving the data problem.

**The Genesis of ImageNet**

Well, first of all, Diana, Gary, and everyone, thank you for inviting me here. I'm excited to be here because I feel like I'm one of you—I'm also an entrepreneur right now, having just started a small company.

ImageNet was indeed pioneering work. We actually conceived it almost 18 years ago—time really flies. I was a first-year assistant professor at Princeton, and the world of AI and machine learning was so different then. There was very little data available. Algorithms, at least in computer vision, simply didn't work. There was no industry presence, and as far as the public was concerned, the word "AI" didn't even exist.

But there was still a group of us, starting from the founding fathers of AI like John McCarthy, continuing through people like Geoffrey Hinton—we all shared this AI dream. We really, really wanted to make machines think and work. My personal dream within that broader vision was to make machines see, because seeing is such a cornerstone of intelligence. Visual intelligence isn't just about perceiving—it's really about understanding the world and acting within it.

I was obsessed with the problem of making machines see. As I obsessively developed machine learning algorithms at that time—we tried neural networks, but they didn't work; we pivoted to Bayesian networks, support vector machines, whatever was available—one problem always haunted me: the problem of generalization.

If you're working in machine learning, you have to respect that generalization is the core mathematical foundation and goal of machine learning. To generalize, these algorithms need data. Yet no one had data at that time in computer vision. I was part of the first generation of graduate students who started dabbling in data because I was among the first generation to witness the big internet revolution.

Fast forward to around 2007: my students and I decided we had to take a bold bet. We believed there needed to be a paradigm shift in machine learning, and that paradigm shift had to be led by data-driven methods. Since there was no data, we thought, "Okay, let's go to the internet, download a billion images—that's the highest number we could conceptualize—and create the world's entire visual taxonomy." We would use that to train and benchmark machine learning algorithms. That's how ImageNet was conceived and came to life.

It took a while until there were algorithms that showed promise. It wasn't until 2012 when AlexNet emerged—that was the second part of the equation for advancing AI: getting the compute power and throwing enough resources at the algorithms.

**The AlexNet Breakthrough**

Between 2009, when we published a small CVPR poster, and 2012 with AlexNet, there were three years where we really believed that data would drive AI, but we had very little signal indicating whether that was actually working.

We did two crucial things. First, we open-sourced everything. We believed from the get-go that we had to make this available to the entire research community for everyone to work on. Second, we created a challenge because we wanted the world's smartest students and researchers working on this problem—that became the ImageNet Challenge.

Every year we released a testing dataset, while the full ImageNet remained available for training. We invited everyone to participate openly. The first couple of years were about setting baselines—the performance was around 30% error rate. It wasn't completely random, but it wasn't great either.

But in the third year, 2012—I wrote about this in my book—I still remember it was around the end of summer. We were running all the ImageNet Challenge results on our servers. It was late one night when I got a ping from my graduate student while I was home, saying we had a result that really, really stood out.

We looked into it. It was a convolutional neural network—it wasn't called AlexNet at the time. Geoffrey Hinton's team called it "SuperVision," which was a clever play on both "super" and "supervised learning." When we examined what SuperVision did, it was actually an old algorithm—convolutional neural networks were published in the 1980s. There were a couple of algorithmic tweaks, but it was quite surprising initially to see such a dramatic step change.

We presented this at the ImageNet Challenge workshop at that year's ICCV in Florence, Italy. Alex Krizhevsky came, Yann LeCun came, and many others attended. The world now knows this as the ImageNet Challenge AlexNet moment. I want to emphasize that it wasn't just about convolutional neural networks—it was also the first time two GPUs were used together by Alex and his team for deep learning computation. It was really the first convergence of data, GPUs, and neural networks.

**From Objects to Scenes**

Following this trajectory in computer vision, ImageNet solved object recognition. Then AI progressed to understanding scenes, with work like Andrew Karpathy's scene description capabilities.

ImageNet addressed the problem of being presented with an image and identifying objects—"there's a cat, there's a chair," and so on. That's a fundamental problem in visual recognition. But ever since I entered AI as a graduate student, I had what I thought was a hundred-year dream: storytelling about the world.

When humans open their eyes—imagine you just opened your eyes in this conference room—you don't just see "person, person, chair, chair, chair." You actually perceive a conference room with a screen, stage, people, crowds, cameras—you can describe the entire scene. That's a human ability fundamental to visual intelligence and critical for our everyday lives.

I genuinely thought that problem would take my entire career. When I graduated, I told myself that if I could create an algorithm that tells the story of a scene by my deathbed, I would have succeeded. That's how I envisioned my career trajectory.

Then the AlexNet moment came, deep learning took off, and when André Karpathy and later Justin Johnson entered my lab, we began seeing signals of natural language and vision converging. André and I proposed image captioning—storytelling through images. Around 2015, André and I published a series of papers among the first to make computers literally caption images.

I almost felt existential—what was I going to do with my life? That was my lifelong goal! It was such an incredible moment for both of us. Last year, I gave a TED talk where I referenced something André tweeted around the time he finished his image captioning work. I had joked with him, "Hey André, why don't we do the reverse? Take a sentence and generate an image." He knew I was joking and replied, "Haha, I'm out of here." The world just wasn't ready then.

Fast forward to now—we all know generative AI. We can take sentences and generate beautiful pictures. The moral of the story is that AI has seen incredible growth, and I feel like the luckiest person in the world because my entire career started at the very end of the AI winter and the beginning of AI's takeoff. So much of my work and career has been part of or helped drive this transformation.

**The Vision for World Labs**

Even after achieving that lifelong dream of describing scenes and generating them with diffusion models, you're dreaming even bigger. The arc of computer vision went from objects to scenes, and now to this concept of "world." You decided to transition from academia to founding and leading World Labs as CEO.

It is kind of wild. The past five or six years have been extraordinary—we're living through such a civilizational moment of technological progress. While computer vision has seen incredible growth from ImageNet to image captioning to image generation using diffusion techniques, we've simultaneously witnessed another extremely exciting development: large language models. In November 2022, ChatGPT truly opened the door to working generative models that can essentially pass the Turing test.

This becomes inspirational even for someone as old as me—it makes you think audaciously about what's next. As a computer vision scientist, I often draw inspiration from evolution and brain science. Throughout my career, when looking for the next North Star problem to solve, I ask myself what evolution or brain development has accomplished.

There's something crucial to appreciate: human language development in evolution took about 300,000 to 500,000 years, being generous. That's the evolutionary timespan for developing sophisticated human language—and humans are essentially the only animals with such complex language capabilities. We could debate animal language, but truly comprehensive language as a tool for communication, reasoning, and abstraction is uniquely human. That took less than half a million years.

But consider vision—the capability of understanding the 3D world, determining what to do in it, navigating it, interacting with it, comprehending it, and communicating about it. That evolutionary journey took 540 million years. The first trilobite developed vision underwater 540 million years ago, and vision set off an evolutionary arms race. Before vision, animals were simple for the preceding half billion years. But once vision emerged, this evolutionary competition began, and animal intelligence started racing forward.

For me, solving spatial intelligence—understanding the 3D world, generating it, reasoning about it, and acting within it—is a fundamental AI problem. To me, AGI will not be complete without spatial intelligence, and I want to solve that problem. This involves creating world models that go beyond flat pixels, beyond language—world models that truly capture 3D structure and the spatial intelligence of our world.

The luckiest thing in my life is that no matter my age, I always get to work with the best young people. I founded this company with three incredible young but world-class technologists: Justin Johnson, Ben Mildenhall, and Christoph Lassner. We're attempting to solve what I believe is the hardest problem in AI right now.

**Why Spatial Intelligence is So Challenging**

This is indeed incredibly talented team—Christoph created NeRF's precursor before Gaussian Splatting, Justin has that systems engineering mind that achieved real-time neural style transfer, and Ben authored the NeRF paper. You need such a crack team because vision is actually harder than LLMs in many ways.

Language is fundamentally one-dimensional—syllables come in sequence, which is why sequence-to-sequence modeling is so classic. There's something else about language people don't fully appreciate: language is purely generative. There's no language in nature—you don't touch or see language. Language literally emerges from our minds; it's a purely generative signal. Of course, you can write it down, but the generation, construction, and utility of language is very generative.

The world is far more complex. First, the real world is 3D, and adding time makes it 4D. Even confining ourselves to space, it's fundamentally 3D, which is combinatorially much harder. Second, sensing the visual world involves projection—whether through your eye, retina, or camera, you're always collapsing 3D to 2D. This is mathematically ill-posed, which is why humans and animals have multiple sensors to solve this problem.

Third, the world isn't purely generative. Yes, we can generate virtual 3D worlds that still must obey physics, but there's also the real world. You're constantly navigating between generation and reconstruction very fluidly. User behavior and use cases vary dramatically—dial all the way to generation, and we're talking gaming and metaverse; dial toward the real world, and we're discussing robotics. But this all exists on a continuum of world modeling and spatial intelligence.

The elephant in the room is data availability. There's abundant language data on the internet, but where's the data for spatial intelligence? It's all in our heads, but not as easily accessible as language data.

These factors make it incredibly hard, but frankly, that excites me. If it were easy, someone else would have solved it. My entire career has been pursuing problems that are so hard they border on delusional—and I think this is the ultimate delusional problem.

**Applications and Future Directions**

The human brain dedicates significantly more neural resources to visual processing than language processing. How does this translate to different model architectures from LLMs?

That's an excellent question, and there are still different schools of thought. Much of what we see in LLMs involves scaling laws—you can essentially brute force self-supervision all the way to success. Constructive world models might be more nuanced. The world is more structured; there might be signals we need to guide the process—whether you call them priors, supervision in data, or something else. These are open questions we need to solve.

You're right about human perception—we don't have all the answers even for human vision. How 3D vision works in humans isn't a solved problem. We understand mechanically that two eyes triangulate information, but even beyond that, we lack comprehensive mathematical models. Humans aren't actually exceptional 3D animals, so there's much to be discovered.

At World Labs, I'm counting on having the smartest people working on spatial intelligence to solve these challenges.

Is it fair to say you're building new foundation models where outputs are 3D worlds? What applications are you envisioning?

I can't discuss World Labs details extensively, but regarding spatial intelligence applications, the use cases are enormous—just like language. From creation (think designers, architects, industrial designers, artists, 3D artists, game developers) all the way to robotics and robotic learning, the utility of spatial intelligence models is really significant.

Many related industries could benefit—marketing, entertainment, even the metaverse. I'm actually excited about the metaverse. I know many people are skeptical because it's still not working, but that's precisely why I'm excited—I believe the convergence of hardware and software is coming.

**Entrepreneurial Journey and Philosophy**

Your transition from academia to founder-CEO might seem sudden to some, but you've had a remarkable zero-to-one journey throughout your life. You immigrated to the US without speaking English as a teenager and even ran a laundromat for several years.

I'm sure you're all here wanting to learn how to start a laundromat! I was 19, and it was born from desperation. I had no means of supporting my family and parents while needing to attend Princeton as a physics major. So I started a dry cleaning shop. In Silicon Valley language, I fundraised, was founder-CEO, cashier, and everything else. After seven years, I exited.

I think the key point, especially for all of you—looking at this audience, I'm so excited because you're literally half my age or even younger, and so talented. Just do it. Don't be afraid.

Throughout my career, even as a professor, I chose several times to join departments where I was the first computer vision professor. That was against much advice—as a young professor, you should go where there's community and senior mentors. While I would have loved senior mentors, when they weren't available, I still had to blaze my own trail.

I went to Google to learn about business, cloud computing, and B2B operations. Then I started a startup within Stanford because around 2018, AI wasn't just taking over industry—AI became a human problem. Humanity will always advance technology, but we cannot lose our humanity. I really cared about creating a beacon of light in AI's progress and imagining how AI can be human-centered, helping humanity.

So I returned to Stanford and created the Human-Centered AI Institute, running it like a startup for five years within the university. Some people weren't happy I ran it as a startup, but I was proud of that approach.

I just love being an entrepreneur. I love the feeling of standing at ground zero—forget what you've done in the past, forget what others think of you, just hunker down and build. That's my comfort zone.

**Identifying Exceptional Talent**

You've advised legendary researchers like Andrej Karpathy, Jim Fan at NVIDIA, Jia Deng who co-authored ImageNet—they all went on to incredible careers. What stood out about them as students?

First, I'm the lucky one. I think I owe more to my students than they owe to me. They make me a better person, teacher, and researcher. Having worked with so many legendary students is truly the honor of my life.

They're all very different—some are pure scientists hunkering down to solve scientific problems, some are industrial leaders, some are the greatest disseminators of AI knowledge. But one thing unifies them, and I'd encourage every one of you to consider this: I look for intellectual fearlessness.

It doesn't matter where you come from or what problem we're trying to solve—that courage, that fearlessness to embrace something hard and go all-in trying to solve it in whatever way you want, is really a core characteristic of people who succeed. I learned this from them, and as CEO at World Labs, I look for that quality in hiring.

**Q&A Session**

**Q: What should a PhD student work on to become legendary like you?**

I want to give you a thoughtful answer beyond just "do whatever excites you." AI research has changed because academia no longer has most AI resources. It's very different from my time—compute power, data, and resources are limited in academia, and there are problems industry can solve much faster.

As a PhD student, I'd recommend looking for North Star problems that aren't on a collision course with problems industry can solve better using superior compute, data, and team science. But there are fundamental problems we can still identify in academia where it doesn't matter how many chips you have—you can make significant progress.

First, interdisciplinary AI is really exciting in academia, especially for scientific discovery. There are so many disciplines that can intersect with AI. On the theoretical side, I find it fascinating that AI capability has completely outrun theory. We don't understand explainability, causality—there's so much about these models we don't understand that could be pushed forward.

In computer vision, there are still representational problems unsolved, and small data is another interesting domain.

**Q: Will AGI emerge as a unified model or multi-agent system?**

I struggle with the definition of AGI, honestly. The founding fathers of AI who gathered in 1956 at Dartmouth—John McCarthy, Marvin Minsky, and others—wanted to solve machines that can think. That's the problem Alan Turing posed earlier. That statement isn't narrow AI; it's a statement about intelligence.

I don't really know how to differentiate that founding question of AI from this new word "AGI." To me, they're the same thing. I understand that industry likes to call AGI something beyond AI, but I struggle with that because I don't know what exactly AGI is different from AI.

If we say today's AGI-ish systems perform better than narrower AI systems from the '70s, '80s, or '90s, that's just the progression of the field. But fundamentally, the science of AI is the science of intelligence—creating machines that can think and act as intelligently or more intelligently than humans.

Without defining AGI clearly, I can't determine if it's monolithic. Looking at the brain, it's one entity you could call monolithic, but it has different functionalities—Broca's area for language, visual cortex, motor cortex. So I don't really know how to answer that question.

**Q: What type of person should pursue graduate school in AI's rapid rise?**

Graduate school represents four or five years where you have burning curiosity—you're led by curiosity so strong that there's no better place to pursue it. It's different from a startup because startups can't be led purely by curiosity; your investors will be upset. Startups have more focused commercial goals. While some curiosity is involved, it's not exclusively curiosity-driven.

In graduate school, that curiosity to solve problems or ask the right questions is so important. Those going in with intense curiosity will really enjoy those four or five years, even if the outside world is moving at light speed—you'll still be happy following that curiosity.

**Q: What's your view on different approaches to open source in AI?**

I think the ecosystem is healthy when there are different approaches. I'm not religious about "you must open source" or "you must close source." It depends on the company's business strategy.

It's clear why Meta wants to open source—their business model isn't selling the model yet; they're using it to grow their ecosystem so people come to their platform. Open source makes perfect sense for them. Another company monetizing directly might have an open source tier and closed source tier.

At a meta level, I think open source should be protected. Open source efforts in both public sector academia and private sector are so important for the entrepreneurial ecosystem and public sector that they should be protected, not penalized.

**Q: How are you solving the spatial data problem for world models?**

You should join World Labs and I'll tell you! As a company, I can't share many details, but we're taking a hybrid approach. It's important to have lots of data, but also quality data—there's still garbage in, garbage out if you're not careful with data quality.

**Q: How did you overcome challenges as a minority in the workplace?**

Thank you for that thoughtful question. I want to be very careful in answering because we all come from different backgrounds, and how each of us feels is very unique. It almost doesn't matter what the big categories are—all of us have moments where we feel like the minority or the only person in the room. Of course I've felt that way, sometimes based on who I am, sometimes based on my ideas, sometimes just based on—I don't know—the color of my shirt, whatever.

But I want to encourage everybody: maybe because I've experienced being an immigrant woman since coming to this country young, I've developed the capability to not over-index on that. I'm here just like every one of you—to learn, to do things, to create things.

**Closing Thoughts**

All of you are about to embark on something or are in the middle of embarking on something, and you're going to have moments of weakness, strangeness, or uncertainty. I feel this every day, especially in startup life. Sometimes I think, "Oh my god, I don't know what I'm doing." Just focus on doing it. Gradient descent yourself to the optimized solution.

---

*We're hiring at World Labs—engineering talents, product talents, 3D talents, generative model talents. If you feel you're fearless and passionate about solving spatial intelligence, talk to me or visit our website.*