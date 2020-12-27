# Questions

Author: shreyashankar

## Technical

### Machine learning

- [x] Can you beat SOTA on a toy dataset by removing mislabeled examples from the train set? See [this paper](https://arxiv.org/pdf/2001.10528.pdf).

- [ ] Is it possible to "breed" the optimal init parameters of a neural network in a somewhat evolutionary way? As an example, consider the [Lottery Ticket Hypothesis](https://arxiv.org/abs/1803.03635) in which there are subnetworks with good weight inits. What would happen if you found multiple sets of lottery tickets in different parts of networks, and initialized one network with multiple tickets? I understand this example might not be a good example because SGD may seek out subnetworks to optimize in overparameterized networks, but I'm interested in evolutionary strategies w/backprop.

- [ ] How do you train neural networks when your input data schema changes without reinitializing the network and retraining from scratch?

- [x] Which layers of neural networks "forget" first when fine-tuning on a new dataset? See [this paper](https://arxiv.org/abs/2007.07400), which shows that deeper layers are the source of catastrophic forgetting. 

    - [ ] Can you have different learning rates per layer and hope that prevents catastrophic forgetting? 
    - [ ] In a replay buffer, can you replay IR (intermediate representations) instead of the original input?
    
- [ ] Suppose you trained a model from the GLM family to learn a distribution (say, Gaussian, for some fixed mu and sigma). In inference, you vary mu and sigma slightly over time. How will your model performance degrade over time? What if you used a neural network?

### Systems

- [ ] Why, in Kubernetes, do we we typically have one pod per machine?

- [ ] How do you design an event-based PL for deep learning, rather than current polling-based alternatives (i.e. printing out loss every few iterations, monitoring curves until it converges, etc)?

- [ ] How do design more imperative PLs for generating features on large datasets? On one hand, you can generate them with SQL or Spark, but that gets annoying and hard to maintain.

## Mental health

- [ ] Why is it so hard for humans to perform [radical acceptance](https://www.dbtselfhelp.com/html/radical_acceptance_text.html)?

- [ ] How do you determine a human's mood without asking them to self-report?
