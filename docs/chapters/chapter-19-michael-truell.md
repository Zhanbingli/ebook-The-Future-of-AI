# Michael Truell: Building Cursor At 23, Taking On GitHub Copilot & Advice To Engineering Students

**Date:** September 3, 2025  
**Source:** [Youtube](https://www.youtube.com/watch?v=TrXi3naD6Og)

---

## The Genesis of Cursor

We realized we were genuinely excited about the future of coding. Taking a step back, if we were being consistent with our beliefs, there was going to be an opportunity for all of coding to change in the next five years—for all of software development to flow through models. It felt like no one working in the space at the time was really taking that seriously. They had great products and were making them incrementally better, but they weren't aiming for a world where all of coding as we know it today gets automated, where building software ends up looking fundamentally different. With that in mind, we set out to work on exactly that.

## Early Beginnings: From Mobile Games to Robot Dogs

Let's start with the origin story. You have to go way back to middle school when I was reading Paul Graham's essays. Early on, I'd been interested in starting a company for a long time, along with many other pursuits. I actually got into programming through a commercial interest—the first time I ever saw code was over a winter break when my brother and I wanted to create a hit mobile game.

We didn't know how to do that, so we Googled "how do you create a game?" We learned we needed to download Xcode. We did, and were immediately confronted with these bizarre, colorful, esoteric symbols—Objective-C, which is still around but perhaps less popular now for good reasons. We stared at this impenetrable wall of Objective-C, and my brother promptly gave up on programming. He's now on a very different career path, trying to paint or something like that.

But I kept going, bought a book on Objective-C, and eventually started working on mobile games. That was my genesis into programming. Along the way, I was also a big fan of PG's essays, Sam's essays, and many of the YC folks—definitely a major inspiration even from the early stages of high school.

## The AI Journey Begins

I was fortunate to find programming early and become interested in AI early on, with some great collaborators to work on AI projects with. After the foray into mobile games—where I wasn't very good—one thing I built that got popular was actually the technically easiest: a mobile app where you could spoof high scores in games like Piano Tiles and Flappy Bird, then send them to your friends. That went viral. It wasn't the painstakingly hand-crafted game engine—maybe a lesson in startups that code isn't everything.

Soon after, a friend and I became interested in building a robotic dog. We thought it would be great to have a robot you could teach without programming it—give it positive and negative feedback like training a dog. You could give it a "treat" for good behavior or say "bad" for poor behavior, maybe teach it to play fetch.

That idea really animated us, but we had no idea how to build it. So we started where anyone would: Google. This led us down rabbit holes into genetic algorithms, then neural networks, and eventually to reinforcement learning, which even back in 2015 had been worked on for a long time.

We did eventually build a couple of robots—nothing substantial that lasted, but interesting work at the time on making reinforcement learning algorithms more data-efficient, better at learning from very few data points (tens of data points) and from noisy human-provided data. We built a multi-axis robot arm that could swing a paddle and play ping pong, and a Kiwi drive robot we taught to follow lines.

**Interviewer:** So you implemented your own neural network from scratch when you were 16 or 17?

**Michael:** Yes. The constraints were that we were dealing with microcontrollers, which have very little memory and couldn't fit standard ML libraries. As part of our bike-shedding attempt to build a robot dog, we implemented our own tiny neural network library. I have memories of not really understanding the internals or calculus, but fumbling our way through re-implementing important neural network concepts. It taught us a lot, though there were fundamental gaps that took years to fill in later.

## The False Starts: CAD and Messaging

Fast forward to founding Anysphere in 2022. The genesis of Cursor was actually in 2021. My co-founders and I had been interested in AI for a long time. Each of us had our own "robot dog moment"—one co-founder worked on trying to build a Google competitor using LLMs in 2021, training his own contrastive models. Another worked on computer vision in academia. Some of us worked on recommendation systems at companies like Google.

In early 2022, we went on basically a month-long hackathon, hacking on ideas related to picking an area of knowledge work and building what it would look like as AI matured.

**Interviewer:** You collected a lot of data for that first idea, right?

**Michael:** Yes. The first real idea we worked on for months was in mechanical engineering—trying to build a co-pilot for mechanical engineers, training models to predict what you'd do in CAD systems like SolidWorks or Fusion 360, where mechanical engineers model parts in 3D.

We picked it because we thought it would be boring, sleepy, and uncompetitive—doing an armchair MBA analysis. It was a horrible choice from the get-go because none of us were mechanical engineers, and the science wasn't ready for that area.

Much of the work involved data scraping—trying to get all the CAD models on the internet. There were different file formats to convert into something canonical, because CAD is a fragmented software market with many popular systems. Cloud CAD systems don't have easily exportable files and don't want you scraping. The training infrastructure for modeling work was also pretty rudimentary then.

We were simultaneously working on other projects. Two co-founders worked on an end-to-end encrypted messaging system. One had a background in security research, and the idea was that apps like Signal and WhatsApp encrypt message bodies but don't hide who's talking to whom and when—crucial information if you don't want to trust the messaging app provider. If a journalist is talking to a government informant, just knowing they're communicating is really significant information.

**Interviewer:** So you worked for about six months on these ideas and shipped products. How many users did you get?

**Michael:** All these projects were polished and had basically no users.

**Interviewer:** At what point did you realize the ideas weren't working?

**Michael:** It was different for each project. For the messaging system, it was technically impressive but had bad trade-offs—it wasn't scalable. They tried giving it to people, and it didn't work. They tried selling it B2B, and that didn't work either.

For the CAD idea, after months of trying to get traction and make the models useful for end users, we had to reckon with whether we were really interested in these areas or if there was something we were inherently more excited about.

## The Pivot to Code Completion

**Interviewer:** There was a moment you decided these ideas weren't working and had to pivot again. You went through three, four, five ideas before landing on code completion?

**Michael:** Yes. We'd been inspired by tools like Copilot early on but avoided working on AI and coding because we thought it was too competitive then—and it's still competitive now. In 2022, GitHub Copilot was already making about $100 million in revenue, maybe more.

**Interviewer:** And you thought, "We could still do a better job than GitHub Copilot," even though people thought the game was over?

**Michael:** We didn't think we could at the start. It was the desperation of having worked on ideas for a while without being excited about them and having them not work out. That shapes what you care about and aim for.

We realized we were genuinely excited about the future of coding. We also got to see how others in the space were working on their products and how the technology was developing. Taking a step back, if we were consistent with our beliefs, there would be an opportunity for all of coding to change in the next five years, for all software development to flow through models.

No one working in the space seemed to be taking that seriously. They had great products and were making them better, but they weren't aiming for a world where all coding as we know it gets automated, where building software looks fundamentally different. With that in mind, we set out to work on that.

**Interviewer:** That was bold, deciding to stop working on other ideas you didn't have backgrounds in and tackle programming despite the giant Goliath that was GitHub Copilot.

**Michael:** It didn't feel bold at the time—just a bunch of people sitting in their living room with laptops. It's not like pivoting some giant company. Initially, we waded in thinking maybe we'd do a very niche tool for security reviews, detecting future CVEs in code, or build something for one niche area of software. We thought about building specifically for quants and prototyped things just for quantitative researchers.

But in doing that, we were brimming with ideas for what Cursor could be if it were just about being the best way to code with AI in general. We had tremendous conviction and excitement about that, so at some point we decided to go for it.

## Building the First Version

**Interviewer:** That was the end of 2022 when you made that decision. How quickly did you ship the first product, and what did it look like?

**Michael:** It took us about three months from first line of code to opening it up and launching it. Originally, we built our own editor "from scratch"—though it used open-source building blocks like CodeMirror, language servers, and other great primitives that help you build an editor.

**Interviewer:** Oh my god.

**Michael:** We cobbled it together from scratch with our own version of remote SSH, our own copilot integration—since we didn't have autocomplete initially—our own theming system, language server integrations. There's just so much that goes into something as developed as the code editor market to make something competitive that can serve as someone's daily driver.

It was four weeks until we built something we could use as our daily driver, maybe four weeks later until we gave it to first beta testers, then another four weeks before we launched it publicly. It was still very crude at the time—it didn't feel like a big thing to open it up to the public.

**Interviewer:** What did you learn from that first version before you did the forking?

**Michael:** We had the fear of God in us—people hadn't really liked some things we'd built for a while, so we were all-in and very focused.

We learned the first initial set of AI features. When we started, there was just one key command that pulled up this universal remote in the editor. You'd ask it to do something, and the AI would figure out what you wanted—a chat response, a code suggestion you could accept, searching your codebase to answer a question, spinning for a long or short time. There wasn't much control.

Given the technology at the end of 2022, we learned the form factor had to look different. We developed the first early AI features that became part of Cursor's core through iteration for ourselves and beta testers.

Another thing we learned: we were rapidly building a feature-complete version of what we wanted in a normal code editor plus AI stuff we thought was great. But a feature-complete code editor for the world is a much, much longer road. VS Code had been developed over 12 years, was one of the earliest TypeScript projects, had lots of people working on it. We thought we could spin up something equivalent in a few months—we learned rapidly that wasn't reality. Our time would be best spent focused on AI stuff.

Similar to how browsers often base themselves off Chromium's rendering engine, we switched to being based off VS Code.

## Model Training and Early Growth

**Interviewer:** You also implemented your own models, getting inspiration from Codex, right?

**Michael:** When we first raised funding for the mechanical engineering idea, we needed money from the get-go to do model training because off-the-shelf models weren't good enough. One paper we'd reference was the original Codex paper. By our calculations, Codex—the first autocomplete model behind GitHub Copilot—didn't cost that much to train. Even in early-to-mid 2022, when people talked about expensive AI model training, I think it cost about $100k in training costs.

During our mechanical engineering phase, we'd done our own training. When we started on Cursor, we were a bit burned by that experience, so we wanted to be as pragmatic as possible and not reinvent the wheel. We started by doing none of that.

Over the course of 2023, dialing in the product, that ended up being a really important product lever, especially as we scaled and got more users. Having product data to make the product better became a really important muscle to build in the company.

## The Uncertain Year: 2023

**Interviewer:** What happened in 2023? You were still not sure whether Cursor would be a thing, still debating with co-founders about pivoting. It took a long time to get to revenue, right?

**Michael:** Throughout 2023, it was growing, but the numbers were small. We were working on something where there wasn't always a clear next step. 

In some markets, you're well-served by immediately talking to people, listing their problems rigorously, systematically thinking through each problem and direct solutions, prioritizing them. But we were in a different space. We're an end-user application without much complexity budget, trying to build the best way to code with AI. Much of that involves figuring out what you can actually do given today's tools.

You could write down many useful things, but figuring out how to build them and all the details—it's not entirely clear how to move forward.

There were many times throughout 2023 where, if you followed the gradient of exactly what our early users wanted, you'd get pulled in different directions than where we ended up. We had a loud segment of users who didn't know how to code at all—we discussed whether to focus on them. We had users wanting very tech-stack-specific things, building for one technology and making it less horizontal. We resisted that too.

There was lots of early prototyping and wandering in the desert in 2023, figuring out where it made sense to build not just software but our own models to improve or replace API models—like for our tab completion and next edit prediction.

## The Explosive Growth: 2024

**Interviewer:** You went from zero to $1 million around 2023, and it took a lot to get there. Then 2024 was crazy—you went from $1 million to $100 million in one year, growing 10% week over week. How did that happen?

**Michael:** The numbers felt small early on, then the compounding continued. I think a couple of things drove our growth. We're in a market where if you make the product better, you see it in the numbers immediately—things start growing more.

We felt it when we first made Cursor codebase-aware, when we first started predicting your next action, when we made that more accurate, faster, more ambitious—predicting sequences of changes. When we let the AI model take more action within your codebase and do that really fast, speeding it up. All along the way, we focused on making the product better, and the compounding continued.

I don't think this is true of all markets, but we're in a market where end-user preferences matter a lot. If you make the best thing, people hear about it and talk about it. That kept going for a long time.

**Interviewer:** I remember seeing a big shift in YC companies. In 2023, maybe single-digit percentage used Cursor, then in 2024 it was like 80%. It spread like wildfire among the best builders, got onto their Twitter feeds. Was that where most adoption came from?

**Michael:** In the very early stages when launching the editor, we tried evangelizing it on social networks. One of my co-founders, when the dopamine hit was keeping him going in 2022 during our ill-fated ideas, started posting on the internet. He explicitly set out to gain followers not through normal social media tactics but by talking about AI.

It was surprising how someone could read all the papers, think deeply about what was happening, talk about it publicly, and get recognized by influential people in the space. There was this particular open-source model, Flan-T5, that multiple AI efforts ended up using after learning about its benefits directly from my co-founder's Twitter posts. He became a very niche San Francisco micro-celebrity and would evangelize the product early on.

We had this movie-magic demo when we first launched and did a waitlist for our initial user batch. That was helpful getting us kickstarted. But after that, we stepped away and lived like monks in 2023, just focusing on the product. It really spread through word of mouth.

I remember team members saying, "Guys, the product's already good enough. Let's set it aside and focus on growth engineering." We'd do two-month sprints on that, but it just washed away compared to the other work we did that year.

**Interviewer:** By 2024, how big was the company?

**Michael:** It was pretty small in 2023. My co-founders are fantastic engineers, and there were four of us, so we could go pretty far without hiring anyone. We also had our own missteps figuring out the first people to hire and how to do that. We were both very patient early on and focused on hiring less than we probably should have. We ended 2023 with single digits—less than 10 people.

## Vision for the Future of Coding

**Interviewer:** Shifting gears, what are your thoughts on how the future will look with coding?

**Michael:** We've always been this middle-road bet. When we started and were hiring our first people, we'd get weird looks about why we were working on this. At the end of 2022, before ChatGPT happened and the world woke up to these things in early 2023, people thought working on AI was kind of weird, not entirely convinced it was a good use of time or that there would be many great applications.

Even people interested in AI were focused on optimizing the existing form factor, making those products incrementally better. Meanwhile, in our social and professional circles, people were thinking, "Why work on anything other than AGI? All your current work will be obsolete in one or two years."

We've always believed there will be incredibly valuable things to build over the next couple of decades. AI will be transformative—maybe more than any recent technological revolution—but it will take decades. It's going to be an industry-wide effort where independent capabilities each need to develop to reach the end state of transforming software building or other areas of knowledge work.

Concretely, in the near term, we think that for professional engineers—our end users—code is still really important. There will be this long, messy middle where you'll work with AI more and more as it becomes like a colleague, maybe even an advanced compiler that can hide some code from you. You'll still need to read the logic, review it, and edit it.

## Advice for Aspiring Engineers

**Interviewer:** What skills will still matter? What should people study or stop studying?

**Michael:** Programming, like math, is just good general education, and I don't think that goes away. There are lots of practical skills from studying computer science. Often when people enter dynamic industries, the specific stuff they study in school isn't super crucial—it's more the learning they get along the way. I don't think that's changed with AI.

**Interviewer:** What advice do you have for a young Michael Truell three years ago, before starting Cursor?

**Michael:** Just work on things you're interested in, and do it with people you both enjoy being around and respect tremendously. Take that really seriously.

For many people in school, so many things pull you toward checking boxes rather than focusing on building something up over time and really focusing on something you're interested in.

**Interviewer:** All right, let's give it a round of applause to Michael. Thank you so much.

**Michael:** Yeah, of course. Thank you for having me.