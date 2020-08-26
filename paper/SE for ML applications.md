## Software Engineering for Machine-Learning Applications(The Road Ahead)

Relevencies:

[Paper's link](https://ieeexplore.ieee.org/document/8474484")

- The need and desire are two main reasons for breakthrough is ML and AI
- The problem is how to effectively develop, test and evolve systems while there isn't complete specifications or source code corresponding to some of their critical behavior.
- The main reasons for failures and shortcomings are shift in the development paradigm induced by ML and AI

- ### System Accuracy:

- The learned behavior of an ML-based system might be incorrect, even if the learning algorithm is implemented correctly, a situation in which traditional testing techniques are ineffective.
- There are three area of AI resaerch:
    - Building programs that imitate human behavior to better understand human thinking (used in
      psychology, research)
    - Building programs that play games well (challenging and fun)
    - Demonstrating that practical computerized products can use the same methods that humans
      use (risky and often naive)

- Turing did not claim that his test was a test for artificia intelligence!
- AI’s goal is not to achieve 100 percent accuracy because:
    - humans are also far from 100 percent accuracy in their daily tasks
    - AI technology’s strength comes from the ability to abstract up from different factors of       variation between environments, to obtain models that can generalize and transfer to situations that weren’t encountered before.

- AI technologies’ main challenge is the curse of dimensionality that is, the need for sufficient, labeled data to cover all important factors (features) of a given problem. AI, in fact, needs
more training data than humans do!
- Key properties of techniques such as deep learning (for example, compositionality, encoding
into a simpler domain, and conditional computation) aim to reduce dimensionality’s impact.
- Engineers are responsible for protecting the public and should release the AI technologies that are harmless and public should be accurately informed of the technology.
- AI isn’t a panacea,the blind application of AI wouldn’t improve the workflow of workers.

- ### System Testing

- When there is no clear specifications of the intended systems exist, AI can approximate the system’s intended behavior by learning models from the available data.
- This model, pushes most of the risk toward the trained models’ quality
- We can use AI technology to reduce the search space of the environments to be tested, nudging
QA techniques to those environments most likely to have failures or violate important safety constraints
- Hardware systems should incorporate fault-tolerance mechanisms to cope with such failures.
- Hardware could incorporate fault-tolerance mechanisms to mitigate the effect of AI model errors, improving AI systems’ robustness.
- Another major challenge is that humans, once they’ve started trusting AI in their daily tasks, could begin adapting their behavior to the AI assistance.
- Humans are essential for putting the decisions of AI into context, so they won't be obsolete once AI technologies become mainstream

- ### Industrial Applications

- Open problems and what they consider to be their biggest needs and top priorities are:
    - There are several programming-language issues involved in ML libraries, models, and frameworks

- ### Healing the Rift

- Unfortunately, a rift exists between these ML and SE. One reason is stakeholders in the AI community focus on algorithms and their performance characteristics, whereas stakeholders
in the SE community focus on implementing and deploying those algorithms.
- Test is intersections between ML and SE.
- The notion of coming up with ways to break a system is integral to ML.
- Missing test cases that are known to fail (but are rare) are a larger issue for ML than for regular software systems.
