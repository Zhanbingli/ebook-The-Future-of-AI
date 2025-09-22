# Aravind Srinivas: Perplexity's Race to Build Agentic Search

**Moderator:** Aravind, I see you every two or three months and you give me an update on the latest at Perplexity. Why don't you tell these folks where you're at? How are things going? Do people actually use Perplexity?

**Aravind:** Whether you believe it or not, I have infrastructure issues every single day. There are a lot of people using Perplexity, and this usage is growing to the extent that we don't actually know how to deal with it. We have to rebuild our infrastructure to scale the next 10x. So there are definitely a lot of people around the world using it—thanks to all of you as well.

What's next for us? The browser. That's the big bet we're making for the future of the company. Everyone here asks: why should I use Perplexity when there's Google search and other AI apps? Of course, ChatGPT has bigger distribution than us. Every other AI app is trying to add search as a layer. All of them support citations. Many support some of the verticals we've put work into. Yes, we'll always continue to remain better than others in that category, but I think the browser and agents are truly the next bet we want to make.

We think about it as an assistant rather than a complete autonomous agent—one omnibox where you can navigate, ask informational queries, and give agentic tasks. Your AI is with you on your new tab page, on your sidebar, as an assistant on any web page you visit. This makes the browser feel more like a cognitive operating system rather than just another browser.

We hope to make it like a cloud where you launch several tasks in parallel that run asynchronously, pulling all your personal contacts, email, calendar, Amazon, and social media accounts. You can do research on real estate or markets—these are all processes running on your browser. That's never been possible before. Chrome was exciting when each tab was its own process. Think about each query or each prompt being that—that will be our new browser, Comet. We're putting all our energy into that.

**Moderator:** This was going to be the hard question I saved for the end, but since you brought it up, I'll ask it now. I think if Sam Altman were on stage today, he would say, "Oh yeah, that's what we're doing." Sundar at Google would probably say that's the direction they're headed as well. It feels like there are many well-funded players going in generally the same direction. How do you see the world? Do you think there will be different use cases where you can own an important one that others won't want, or are we in for a major competitive battle?

**Aravind:** Look, if something is really worth doing, it's only natural that people with significant funding will pursue it. People said Perplexity was a great product. Now everyone is trying to build something that can answer any question with sources. Cursor was a great product. Now OpenAI is trying to acquire Cursor's competitor. Anthropic launched Claude Dev. Google has its own rival tool. It's natural that when there's money to be made in a sector, people will try to copy it.

There's only a limited number of things you can be world-class at—whether it's building great models or one or two really good products. You're obviously not going to win at everything. For us, this is the only thing we care about: accuracy at the level of answers, accuracy at the level of tasks, orchestrating all these different tools. The browser is much harder to copy than just another chat tool.

That said, I'm fully operating under the assumption that OpenAI will build its own browser. Anthropic will try to build its own browser. Google already has one called Chrome. It's completely reasonable to expect them to do this. The only mode you have is speed. You have to innovate. You have to move faster than everybody else. It's like running a marathon at extremely high velocity.

**Moderator:** I really agree with your statement that you can only focus on one thing and be world-class at it. To give you folks a glimpse: we were backstage before this talk, and he was showing me some new features they're working on. There was a bug, and he stopped everything he was doing to figure out what was wrong. If you think about what the CEO of a large company would do in that situation, they'd probably hand it off to someone else on their team. That's good evidence that you actually mean what you say.

**Aravind:** I love triaging and fixing bugs. I know it sounds trivial—is that the best use of a CEO's time? Many people would think otherwise. Recently, I've noticed that even Sundar is doing bug support on X right now. I'm happy that behavior is setting a good example.

**Moderator:** Let's go back to the beginning. Most folks in the audience are either students, recent graduates, or grad students. Hearing your story of how you started Perplexity would be really interesting to them because it's probably exactly the world they're in now.

**Aravind:** We started the company without actually having a clear idea of what to build—which is the opposite of what YC advises, which is to start from a problem and turn it into a company. I really think at this point, when AI is improving so fast, you don't have to rigidly stick to any one idea when getting started. But the most important thing is not changing the idea every week either.

Start with something. Brainstorm, think about it, then immediately build it and get it in people's hands. One tool we were building was natural language SQL, which we thought about as a search tool for relational databases. I loved Twitter search—like the original Facebook Graph Search when I was much younger. I wanted to rebuild that using language models.

I love Twitter as a platform, and there's no good way to search over Twitter—there still isn't. We organized Twitter's entire dataset as relational tables and converted every user query into a SQL query, running it against the database. It was really good, and that's what got us started.

At some point, we figured it would be better to scale this across the web. We couldn't make every website into tables, and it's not easy to answer all sorts of questions that way. We bet on the fact that language models could do all the reasoning, parsing, and structuring later. The more important thing was to start with something more unstructured—that ended up becoming Perplexity.

**Moderator:** Maybe one step before you left to start the company—how did you find your co-founders? How did you decide that machine learning and AI was the area you wanted to focus on?

**Aravind:** Because that was the only thing I was good at. I wasn't good at anything else. What's the point of starting a company in an area where you're not the right fit? I couldn't start a delivery company or social media company. The only thing I knew was AI and machine learning.

It's funny—we started an AI company, but we're not training our own foundation models. We train many different models, but that's the extent to which you need intellectual humility to know what you're good at and what's actually doable with the resources you have access to.

My co-founders are people I knew from grad school. We'd been talking and discussing ideas for a long time. Grad school is a great way to identify co-founders. You don't talk to them with the long-term calculation of "this could be my co-founder." You talk to them because they're interesting people. I think that's the value of the Y Combinator network too. Even if your first startup fails, you get access to amazing people who might be your future co-founders.

**Moderator:** You launched this first version of Perplexity for Twitter search. At what point did it start to work, and you internally felt like, "We should keep working on this"?

**Aravind:** Whoever we gave early access to was very excited about it. They kept using it repeatedly. There's a phenomenon in products where there's an initial wow factor. Then it either drops completely—meaning you never had real retention—or it drops but there's sustained usage.

When we saw sustained usage for the relational database searches like Twitter, LinkedIn, and GitHub, we knew there was something magical about combining large language models with search. We dreamed bigger and said, "What if we just give answers and cite the relevant sources?" We launched that as a Discord bot, and that was also continually being used—not just one-day usage where people started ignoring it.

That's when we had the courage to launch publicly. We launched seven days after the ChatGPT launch, especially when ChatGPT didn't have web search. That was good timing. Many successful AI products that people talk about today—Cursor included—were all 2022 launches or early 2023 launches. They're all "old" in AI time scale.

For me, the aha moment was New Year's Eve when we had close to 700,000 queries. I thought, "This has the crappiest name for a consumer product—'Perplexity.' Very hard to pronounce. Nobody knows how to spell it." It was so slow, taking seven seconds to answer a query. It was making mistakes and hallucinations. We were a no-name company with a no-name founder and only two million dollars in seed funding.

Despite all that, people cared enough to share screenshots on New Year's Eve when they could be watching Netflix. That's when I knew there was something real here, and I started optimizing and committing to this vision.

**Moderator:** At that point, did you think you were building something that could really compete with Google and take over a market as big as what Google offers, or was it just a toy?

**Aravind:** The first time that thought occurred to me was when Google wrote a blog post—when Sundar wrote about Bard. This was around when we were raising Series A funding, and everyone said, "Bard is going to do whatever you're doing. Why do you have to build a separate product? Why not just do it on Google where you have all the distribution in the world?"

I kept thinking it was obvious you cannot—if people can get direct answers to questions like "best hotels to stay in San Francisco with a view of the Golden Gate Bridge" or "where can I stay in New York next to Central Park with good amenities," with booking links right there, how are you going to make money from Booking.com, Expedia, and Kayak? They're all bidding against each other for the same ad space. It's not in their incentive to give you good answers at all.

That's when I realized Google would have to build a separate product, but they could never capitalize on their core distribution. In 2023 and much of 2024, Google had maybe the fourth or fifth best models at any moment. As a startup outside Google, you had access to AI that was better than what Google internally had—which was unprecedented.

Until then, if you had to compete with Google on something requiring AI, good luck, because you never had AI outside Google that was even equal, let alone better. Now it's a complete reversal thanks to OpenAI, Anthropic, and open-source models.

Plus there's the innovator's dilemma and the fact that we could make many mistakes and it's fine, whereas for Google, one mistake tanks their stock. Remember the live demo of Bard where it failed and the stock went down 6%. We knew there were many advantages for us.

**Moderator:** You've talked about how Google has been trying to build Perplexity-like experiences—AI Overview, now AI Mode. You mentioned they just change the name each Google I/O.

**Aravind:** It might sound a little cocky to say, but it's true. The same feature is being launched year after year with a different name, different VP, different group of people. It's the same thing—maybe getting better—but never getting launched to everybody.

**Moderator:** One thing I've come to admire about you is your focus on user experience, which you learned from Larry Page by reading about Google. Why do you think Google has lost that ability?

**Aravind:** It's a much bigger business now, and it's not founder-led anymore. It's hard to take risks. They have great people—nobody would think Google has incompetent people. They have really great engineers. It's largely the incentive structure. It's hard to take a hit on your stock and do what's long-term correct.

Honestly, I'm happy that dilemma exists because otherwise, where's the opening for startups? If startups couldn't succeed, it would just be monopolies getting bigger, and that's not great for the world.

I'm happy we can win and they can ship new products, and people are comparing for the first time. Earlier, for access to information, you would never bother to compare an alternative to Google—that was considered a waste of time, a joke. Now at least you think, "I'll ask this app, I'll ask Google, I'll ask ChatGPT, I'll ask Perplexity, I'll ask Gemini," and maybe you don't even ask Google anymore.

**Moderator:** You were telling me backstage that despite increased competition, you haven't really seen an effect on your numbers.

**Aravind:** I read all the Twitter comments every time. Google I/O last year was "AI Overview and Perplexity is dead." This year was "AI Mode and Perplexity is dead." I read all of that too, and it's always fun—I love it actually, because they know they're thinking, "Google wouldn't build this or something," but the reality is nobody actually gets exposed to those features.

But competition is real. Let's accept that OpenAI is extremely well-funded, doesn't have innovator's dilemma problems, and wants to ship search on ChatGPT. ChatGPT is the most successful consumer AI product out there. Competing against it is very difficult, which is why I want to push the company more on the browser side.

I think Comet, our browser, will be an abstraction layer above chatbots. You could even imagine if you permit Comet, all your ChatGPT chats could be fed into that AI. You don't have to worry about memory or personalization, and it'll do things a chatbot cannot do—like accessing other tabs, accessing your browsing history, completing forms for you, paying your credit cards, buying stuff for you, being your scout, doing research, handling periodic recurring tasks. That's the magic the browser enables.

Putting this into mobile and building mobile versions will be very hard engineering-wise—it'll take many months. I'm not really worried about someone else trying to copy this quickly.

**Moderator:** Switching to a different browser is a pretty big decision for users. What are the very short-term things your browser will do so much better than Chrome that will make me want to switch?

**Aravind:** The perfect blend of AI, navigation, and agents is what we're going to offer. It might sound like a boring answer, but no one's done that. There are hundreds of millions, probably close to a billion people using AI these days, so the market's already pretty big.

**Moderator:** What's a specific example of how I would use that if I had access tomorrow?

**Aravind:** You can schedule your meetings. You can reply to emails you don't even want to read. For example, let's say you're hosting a Y Combinator event and you say, "I only want to accept Stanford dropouts." It can go through the entire list of applicants, scrape their LinkedIn URLs, filter based on whether they went to Stanford and whether they dropped out, then accept accordingly. That level of multi-step reasoning is something you can uniquely do.

By the way, I'm not saying that's a good filter—I wouldn't get in otherwise, so hopefully you're more open. We look for DeepMind researchers also.

**Moderator:** Let's talk about how you run the company now. You have about 200 employees. You now have access to code-writing AI tools. Are you guys all-in on that stuff? What does it look like?

**Aravind:** You don't want to AI-code everything. We frequently run into infrastructure issues, and you don't want an AI coder fixing live things in production. I want people well-trained in regular software engineering, infrastructure, and distributed systems—you don't want to replace these skills.

But for front-end design, we're seeing tremendous adoption. Cursor is being used by everybody. We made it mandatory to use at least one AI coding tool internally at Perplexity—it happens to be Cursor and a mix of Cursor and GitHub Copilot.

Machine learning people can read a paper, upload a screenshot of the pseudocode, ask Cursor to edit files to implement the new algorithm, and it can write unit tests and run an experiment pretty quickly. This reduces experimentation time from three or four days to literally one hour.

Sometimes I give feedback by taking a screenshot of my iOS app and saying, "This button needs to move here," with an arrow. They upload my screenshot to Cursor and ask it to write changes to the SwiftUI file. The speed at which you can fix bugs and ship to production is incredible.

But it's also introducing new bugs. Many people don't know how to fix them and don't even know how the bug got introduced. It's not perfect. The newer tools like Claude Dev seem to be far smarter than what Cursor can do. I'm really positive this is the right future, but there are issues right now.

**Moderator:** As these coding tools get better, what's the enduring value of a company like yours if it's increasingly easy to replicate what you've done using these tools?

**Aravind:** Brand definitely has big value. There are Cursor competitors and Perplexity competitors. OpenAI will have their own Cursor. OpenAI has Perplexity within ChatGPT, but that didn't kill any of these companies. There's brand value that, once you acquire at the scale of several million paying users, means you don't die that fast. You earn the right to survive and keep building.

Brand is important. Narrative is very important to the brand—you have to communicate to people why you even need to exist. For us, it's the focus on accuracy. Let there exist 100 chatbots, but we're the most focused on getting as many answers right as possible. We focus on speed—time to first token on app or web. We're still the fastest despite doing search. We focus on how we present the answer.

There are things you're obsessed about because you care about them, and that becomes your narrative and brand identity. If you manage to get reasonable distribution—not 100 million users, but tens of millions—you earn the right to keep playing the game no matter what others ship. Until then, it's definitely a challenge. Even now we worry about it, and the only solution is to move fast and keep shipping.

**Moderator:** Beyond brand, do you think about network effect types of things emerging with Perplexity?

**Aravind:** Brand has network effects—people tell each other about the brand. But no AI product has within-app network effects like WhatsApp, where even though people don't necessarily trust Meta's products and think they're ad products, nobody can easily switch off WhatsApp because all your contacts and groups are there.

AI doesn't quite have that yet, mainly because you can easily export your ChatGPT history and upload it somewhere else. The browser will definitely be one way to figure this out because your browsing history, passwords, wallet, and agent tasks create more stickiness and network effects, especially if multiple people rely on the same set of tasks and share them.

**Moderator:** A lot of what you aspire to solve requires integrations or partnerships with other companies. What does that look like in the future?

**Aravind:** We already work with SelfBook—they power all hotel bookings natively done on Perplexity. We work with TripAdvisor to surface hotel reviews and places. We have collaborations for maps. We work with Yelp. For shopping, we have many merchants selling directly on us, and we work with Affirm to support bookings and native purchases. Shopify is one of our partners. For finance, we work with FMP. For sports, we work with Stats Perform. There are already many data providers working with us on these verticals.

We think it'll expand further as agents start doing things. Different people are okay with becoming MCP servers. Some aren't and want to preserve their websites. The browser agent will be generic enough that it'll respect whatever the third party wants because the agent is being permitted by the user to act on their behalf.

If there's no MCP server, it's still fine—you can use tabs as if the user would have done it. That's the key advantage of the browser versus committing entirely to the MCP vision, where you require third-party MCP servers to work reliably.

**Moderator:** Your main competitor Google's business model is selling ads, which you think prevents them from being really good at what you're doing. What will your business model be?

**Aravind:** I don't know if we'll ever get order-of-magnitude profits like Google—just to be clear, and I don't think that's needed. No one in history, even Google, has had another business with the margins Google has. It's reasonable to get something far better than any public company right now and still be way below Google.

The subscription revenue is really encouraging. We never expected to get this far, and we think we can grow at least a few billion a year in just subscriptions, which is a great business.

Usage-based pricing where people pay an agent for completing a task, or people have recurring tasks and pay based on every single use, normalizing based on what it would cost to hire a person to do that, is going to be a thing. I don't know exactly how it'll play out or what the margins will be. Potentially it'll be way better than subscriptions in terms of volume of people who pay, but might be lower margins because it's usage-based.

If people start buying more through AIs, taking a cut of transactions is good. CPAs have historically been way lower margins than CPCs, which is why Google never became a transaction platform and why you may make good money here but never as much as Google. Google's business model is potentially the best business model ever—it was so good you needed AI to kill it.

**Moderator:** If you were in their position four years ago, what would you advise folks in this room to do?

**Aravind:** Work incredibly hard. There's no substitute for it. Don't think you're very smart and can strategize the right way to build a company despite what big model labs are doing. You should assume that if you have a big hit—if your company can make revenue on the scale of hundreds of millions or potentially billions of dollars—a model company will copy it.

They're really looking for revenue. They raise tens of billions or close to 50 billion and need to justify all that capex spend. They need to keep searching for new ways to make money, so they'll copy anything good. There's only a limited number of things you can be world-class at.

You have to live with that fear. Embrace it and realize your mode comes from moving fast and building your own identity around what you're doing, because users care. When you're searching for a specific person for house help, you search for that specific person—you don't go to a general agency that handles everything.

There's real benefit from embracing that fear, sleeping with that fear, waking up every day feeling excited about what you're going to build, because that's the only thing that'll keep you going.

---

## Q&A Session

**Q: With your recent partnership with Nvidia and potential pre-installation on Samsung phones, what are the most important factors at Perplexity to prevent hallucinations?**

**A:** Hallucinations are something we really care about. We're building benchmarks internally to keep up to date with that. The only way is to keep building a better search index, keep capturing better snippets of all web pages. These models are getting fast enough that you can have them reason multi-step for every query without incurring too much cost, and that's another way to reduce hallucinations.

**Q: If you were in Sundar's shoes, what would you do? Would you sacrifice the business model to get the next product, or ship it as a separate product?**

**A:** I don't envy that job at all. Nobody in the world wants that job—it's very difficult. I genuinely don't know what I'd do. They have more data on what their users are doing. There are many people in the world who hate AI, so throwing AI down people's throats on such massive distribution isn't easy. If ads are part of every AI answer, you're going to hate it too. It's good that there are alternatives like us.

**Q: How would you approach the issue of foundation models consolidating search into their own infrastructure?**

**A:** Pick something you want to be known for. Yes, others are integrating search, but we still want to be the fastest and most accurate. Obviously, I can't just say that and stop—we need to figure out a new strategy and build new products that don't exist yet.

Our browser will be that bet for us. Browser and search aren't two distinctive products—the browser is a natural graduation step from search, just like how Google graduated from Google Search to Chrome. Chrome is the main reason they got billions of daily queries from hundreds of millions of users. When Google IPO'd, they had no browser and maybe 100 million queries. Now it's like 10 billion or something.

**Q: What do you tell yourself when you feel like you might fail?**

**A:** I watch Elon Musk videos on YouTube. No, I'm serious. There's a video where there's a third failure in a row, and when asked what he thinks, he says, "I don't ever give up. I would have to be dead or incapacitated." There are examples of great entrepreneurs who've done this despite all odds stacked against them. What do you have to lose? Just keep going.

**Q: What do you think the web will look like in 5-10 years when AI search engines drive less traffic to websites?**

**A:** The web is already pretty long-tail with massive power laws, and the distribution will get even more skewed. There will be certain well-known brands that preserve direct organic visits, but those trying to game the SEO system will have a harder time.

**Q: How do you deal with political bias in news articles and human-written sources?**

**A:** There are cases where you have objective truth—like NBA game scores or live weather in San Francisco—where you don't want to be wrong ever, and people know what's true. But even there, you're trusting data providers.

For things that don't have one clear accurate answer, the best thing we can do is offer all perspectives and not take a clear opinion on what's right and wrong when there's no clear answer.

**Q: How do you decide which audiences you're trying to reach?**

**A:** Try to get into distributions of users you don't typically have access to through traditional marketing channels. There are many people who don't use Twitter or LinkedIn—we're living in a bubble here. Some businesses have good access to them, like traditional businesses.

The kind of people who use Costco regularly may not be using AI regularly, so if those are the people you're going for, it makes sense to change your strategy. But remember, it's good to grow with adjacencies—you want some overlapping sets of people who'll be word-of-mouth carriers as they help you expand to non-overlapping circles. There should be some overlap, but your distribution should keep evolving over time.s