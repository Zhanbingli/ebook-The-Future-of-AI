# Chapter 3: Intelligence in Motion

*Chelsea Finn on Building General-Purpose Robots*

### Beyond the Single-Purpose Machine

For decades, robotics has been trapped in a paradox: to solve any meaningful problem, you essentially need to build an entire company around that specific application. Want robots for logistics? Build specialized hardware, develop custom software, design unique movement primitives, and handle countless edge cases—all from scratch. The result has been a fragmented landscape where robotic solutions remain expensive, brittle, and limited in scope.

Chelsea Finn and her team at Physical Intelligence are pursuing a fundamentally different approach: developing general-purpose models that can enable any robot to perform any task in any environment. "We're trying to develop a general purpose model that can enable any robot to do any task in any environment," Finn explains. "We think that this sort of generalist model may work better and be easier to use than purpose-built models, just like we've seen in the development of foundation models for language."

### The Data Dilemma

The path to general-purpose robotics faces a crucial challenge that sets it apart from other AI domains: the nature of training data. While language models can train on vast corpora of human-generated text, robotics data comes with unique constraints and trade-offs.

Industrial automation provides massive scale—robots performing the same tasks millions of times. But this data lacks the diversity needed for general intelligence. "This sort of data isn't going to allow robots to go into disaster zones or to make a sandwich or to bag groceries," Finn notes.

YouTube videos offer behavioral diversity, showing humans performing countless different tasks. However, there's a fundamental embodiment gap: "We don't learn how to write by watching other people write, and we don't become expert tennis players by watching Wimbledon."

Simulation can generate unlimited synthetic data, but it struggles with realism and the sim-to-real transfer problem.

The solution, Finn discovered, requires high-quality real-world robot data, even if the quantities are smaller than what other AI domains enjoy. "Scale is necessary for developing these models that can generalize in open world conditions, but it's subordinate to actually solving the problem."

### The Laundry Folding Breakthrough

One of Physical Intelligence's most impressive demonstrations—a robot that can unload a dryer and fold laundry—illustrates both the potential and the challenges of general-purpose robotics. "To date, I think this is the most impressive thing that I've seen a robot do in the physical world," Finn says. "It's really hard."

The task requires handling variability in clothing types, positions, and crumpling patterns while maintaining dexterity over a 10-minute sequence with numerous opportunities for catastrophic failure. The breakthrough came through a counterintuitive insight borrowed from language model development: pre-training on all available data, then fine-tuning on a carefully curated, high-quality dataset.

"We pre-train on all the data and then fine-tune on a curated, consistent, high-quality set of demonstration data," Finn explains. This approach proved far superior to training only on curated data or only on the full dataset without fine-tuning.

### The Foundation Model Advantage

The power of foundation models in robotics becomes clear when considering how quickly new capabilities can be developed. The same pre-training and post-training recipe that enabled laundry folding also worked for entirely different tasks: cleaning tables, scooping coffee beans, constructing cardboard boxes, and lighting candles with matches.

More remarkably, the approach transferred across different robots with minimal adaptation. "They collected data, sent the data to us, we fine-tuned our model on their data... the model is able to control the robot to make a cup of coffee," Finn describes, referring to a collaboration with a robot she had never seen in person.

This transferability hints at the true potential of foundation models in robotics: the ability to amortize learning across tasks, environments, and even physical platforms.

### Scaling Across Environments

Physical Intelligence's approach to environmental generalization demonstrates the power of diverse training data. They collected robot data in homes across San Francisco, in mock kitchens and bedrooms, totaling more than 100 unique rooms. Crucially, this mobile manipulation data represented only 2.4% of their overall pre-training mix, yet it enabled robots to operate successfully in entirely novel environments.

When tested in rented Airbnbs the robots had never visited, the systems successfully performed tasks like closing cabinets, putting away dishes, and cleaning spills. "Quantitatively, we find that if we actually increase the amount of homes, the amount of locations that are represented in the data, the performance increases," Finn reports.

### The Language Connection

One of the most sophisticated aspects of Physical Intelligence's approach involves hierarchical vision-language-action models. The system breaks down complex natural language instructions into subtasks, then executes them through low-level motor controls.

But training such systems faces a data bottleneck: it's impractical to collect massive amounts of human-robot interaction data for every possible command. The solution involves synthetic data generation, where language models create hypothetical human prompts for existing robot behaviors.

"We take data that says here's a video and then the next skill is to pick up a KitKat... we can ask a vision language model, what is a hypothetical prompt that a human might have asked that led to this particular scenario," Finn explains.

This approach enables robots to respond to open-ended prompts like "Can you make me a vegan sandwich? I don't like pickles, though," and handle real-time interjections like "Get me something sweet that's not in the basket."

### The Technical Architecture

Physical Intelligence's technical approach centers on vision-language-action (VLA) models that combine pre-trained vision-language models with action prediction heads. The key insight is preserving the language-following capabilities of the foundation model while adding robotic control capabilities.

"We're going to be predicting tokenized actions, and when we have the diffusion head, we'll be stopping the gradient from the randomly initialized diffusion head to prevent it from deteriorating the language following abilities of the VLM backbone," Finn explains.

This architectural choice proved crucial for maintaining the robot's ability to follow instructions accurately—achieving an 80% success rate compared to just 20% with approaches that didn't preserve the pre-trained knowledge.

### The Integration Challenge

One of the most underappreciated aspects of robotics development is the infrastructure required for real-time control. "We have a real-time system that needs to actually be hitting a certain frequency to actually execute actions successfully," Finn notes. "If you have lag in that system, it introduces all sorts of challenges."

This infrastructure layer—encompassing real-time control, multimodal data ingestion, and large-scale model training—represents a significant engineering challenge that goes well beyond the machine learning components that typically receive attention.

### Lessons from Failure

Physical Intelligence's development process included months of failure that provide valuable insights. When early approaches to laundry folding achieved 0% success rates despite trying various architectural improvements, the breakthrough came from stepping back and applying lessons from language model development.

"We had around two to three months of failure where nothing was really working," Finn admits. The eventual solution required not just better algorithms, but better training data curation and the discipline to maintain focus on a concrete, measurable task.

### The Path Forward

Finn's vision for the future of robotics centers on the continued development of foundation models that can generalize across tasks, environments, and platforms. However, she maintains a realistic perspective on current limitations and remaining challenges.

"There's lots of work to do still," she acknowledges, citing issues with speed, partial observability, and long-term planning. Success rates of around 80% for relatively simple tasks indicate significant room for improvement before robots can reliably handle complex real-world scenarios.

### Implications for Builders

For entrepreneurs and technologists, Physical Intelligence's approach offers several key insights:

**Start with Real Data**: Despite the appeal of simulation or large-scale industrial data, breakthrough capabilities require high-quality, diverse real-world training data.

**Embrace Foundation Models**: The ability to pre-train once and fine-tune for multiple tasks provides significant advantages over building specialized systems from scratch.

**Focus on Concrete Tasks**: Progress comes from tackling specific, measurable challenges rather than pursuing vague goals like "AI for robotics."

**Invest in Infrastructure**: The unglamorous but crucial work of building reliable real-time systems often determines the difference between impressive demos and useful products.

### The Broader Vision

Physical Intelligence's work represents more than just better robots—it points toward a future where intelligent systems can operate effectively in the physical world. This capability could transform manufacturing, healthcare, domestic life, and countless other domains where physical manipulation remains a bottleneck.

The company's approach of starting with concrete tasks while building toward general-purpose capability offers a template for navigating the transition from narrow AI applications to more broadly capable systems. As Finn puts it, "We've seen a few different scenarios in this talk where general purpose robots might be more successful than specialist robots because we can essentially, rather than start from scratch for every single application, actually build upon a much broader foundation for physical intelligence in the real world."

This foundation model approach to robotics may well prove to be as transformative for physical intelligence as large language models have been for digital intelligence, opening up possibilities that we're only beginning to imagine.

------
