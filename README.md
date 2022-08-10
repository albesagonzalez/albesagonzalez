# Welcome to my GitHub profile!

Welcome to my GitHub profile, my name is Albert and here you can find some of my work in the fields of Computational Neuroscience and Artificial Intelligence. If you are curious about what these fields are and how they relate to each ohter, keep reading!

<img src="https://github.com/albertalbesa/albertalbesa/blob/main/figures/what_is_cn.png" alt="drawing" width="750"/>

This sounds (and indeed is) very cool. By creating models that are able to reproduce experimental data, one can make predictions on what should be observed in regions of the model parameter space out of the original experiments solely based on simulations. But it does not stop there... Many years ago, some scientists understood that mathematical models of neurons, especially the simplest ones, could not only be used within neuroscience, but also allowed machines to mimic intelligent behaviour: it was the birth of Artificial Neural Networks (ANNs).

<img src="https://github.com/albertalbesa/albertalbesa/blob/main/figures/anns.png" alt="drawing" width="750"/>

At that point, Computational Neuroscience (CN) and Artificial Intelligence (AI) diverged into two different disciplines: while the first is insterested in understanding the brain, the second intends to achieve artificial systems able to perform complex cognitive tasks. Nevertheless, the two are still related, and keep on influencing each other today. For example, discoveries in neuroscience inspire new algorithms in AI, and fundamental findings in AI guide what could be expected from neural systems, which have been optimized by evolution for hundreds of millions of years.

Since I became interested in these areas, I have participated in different projects. Through this, I have tied to gain knowledge on as many approaches as possible and, as well as finding the specific topics that motivate me as a future researcher. Here is a selection of 4 of them to exemplify my experience:

## Playing BlackJack with Reinforcement Learning

Reinforcement Learning (RL) is inspired in psychology and how agents learn to interact with an environment based on *rewards* and *punishments*. This technique has gained popularity since the release of an iconic paper [Playing Atari with Deep Reinforcement Learninig](https://arxiv.org/pdf/1312.5602v1.pdf), which combined an old-established method (Q-Learning) with Deep Neural Networks (DNNs) to teach an agent how to play computer games based solely on the screen images and taking the achieved score as a reward.

In [this project](https://github.com/albertalbesa/playing_blackjack), which I carried out with two other colleagues, we explored the use of many different techniques in RL to get an agent to learn how to play BlackJack. We developed both the environment and the agent from scratch only using scientific computing packages, without any help from ML packages (like Tensorflow). The techniques used were MonteCarlo, Q-Learning, Deep Q-Learning and Policy Gradient. Furthermore, we used DNNs and also Quantum Variational Circuits as function approximators (functions used to approximate the so-called *action-state value*).


## Weight dependece in BCM leads to adjustable synaptic competition

In standard Machine Learning (ML), one can use a technique called *Gradient Descent* to find in what direction the parameters of a model should change, provided a *Loss Function* that indicates how much the model deviates from *good performance*. In bioloigcal neural networks, this has been argued to be close to impossible, so that alertnative *unsupervised* and *local* learning rules should guide changes in *synapses* (which would be analogous to the weights in ANNs). A classic example of this is the Bienenstock-Cooper-Munro (BCM) rule of synaptic plasticity, which was proposed in 1982 as a model of learning for neurons in the primary visual cortex. As unrelated as this can feel to AI, this model precisely explains how the topology found in Convolutional Neural Networks (CNNs) early layers, which speciallize in finding edges at different orientations, can naturally emerge in the brain.

In [this article](https://link.springer.com/article/10.1007/s10827-022-00824-w) published in the *Journal of Computational Neuroscience*, we studied a variant of this rule that incorporates *weight-dependence*, a biologically-inspired feature observed in real synapses, which have been found to change proportionally to their strength when being depressed. We found that adding this feature establishes a continuum of *selectivity* (or *competition*), which is an indicator of how distinctly a neuron reacts to different stimuli. In our model, this gradient of selectivity is controlled by the ammount of inhibition, which is a negative feedback signal that excitatory neurons receive in response to their own activity. A visual representation of this result can be seen in the following figure (extracted from the original paper), where one can see how inhibiton establishes regions of 0 selectivity, variable increasing selectivity, and maximum selectivity.

<img src="https://github.com/albertalbesa/albertalbesa/blob/main/figures/wbcm.png" alt="drawing" width="400"/>


## Exploring autonomous driving: a Deep Learning approach

Coming back to Deep Learning (DL), this is [an example project](https://github.com/albertalbesa/reports/blob/main/Autonomous_Driving.pdf) that helped me delve into classic techniques in DNNs. This allowed me to gain expertise in ML frameworks such as Tensorflow and PyTorch, as well as in the complete ML pipeline that comprises data processing to inference. The problem was the following: given a set of images taken from a toy car in a 3D printed circuit (see figure below), we had to create a DL architecture able to predict the proper driving commands (which in this case were the steering angle and velocity).

<img src="https://github.com/albertalbesa/albertalbesa/blob/main/figures/example_sdc.png" alt="drawing" width="400"/>

The initial approach was to use an architecture inspired in the [NVIDIA model](https://arxiv.org/pdf/1604.07316.pdf) for end-to-end autonomous driving. This was a nice start and provided with reasonably good performance. However, it was not making use of potentially benefitial pre-processing layers that explicitly identified pedestrians, direction signs or traffic lights. We then included additional models that were trained to do that, using techniques such as image segmentation (left) and object detection (right, includes examples of all true and false positives and negatives). Including this information to the input given to the original NVIDIA architecture assisted and simplified its task to predict proper steering commands.

<img src="https://github.com/albertalbesa/albertalbesa/blob/main/figures/example_cv.png" alt="drawing" width="800"/>


## Paper reproduction: Inhibitory connectivity defines the realm of excitatory plasticity

Finally, I would like to include [a project](https://github.com/albertalbesa/inhibitory-connectivity) that I found significantly empowering to puruse a career in research: a paper reproduction. My colleagues and I were given the task of reproducing the main figures of the paper [Inhibitory connectivity defines the realm of excitatory plasticity](https://www.nature.com/articles/s41593-018-0226-x), building our own simulations from scratch using as guidance the methods section of the paper. The original research work had proposed that inhibitory connectivity (connections from inhibitory to inhibitory neurons) could be sufficient to mantain memories in the brain, even when excitatory connections were eroded. To do this, they used a Spiking Neural Network, in which neurons communicate with each other via *spikes*, so that only at the specific times in which neurons *fire* they send messages to other neurons.

The project was significantly challenging and included autonomously looking for solutions to issues that were not explicitly mentioned in the original paper. However, finally seeing that (albeit with guidance) we had been able to take the steps that such renown scientists had taken before was an amazing sensation. The following is a figure extracted from our report. In the top, the neural networks is able to sustain its activity after a memorized input has been presented. In the bottom, while the network is able to still recover a memory with a complete rewiring of excitatory conncections, it fails to do so if the same is done with inhibitory connections.

<img src="https://github.com/albertalbesa/albertalbesa/blob/main/figures/inhibitory.png" alt="drawing" width="400"/>

## Other work samples

In [this repository](https://github.com/albertalbesa/reports) you can find more samples of work I have done in the past, so feel free to take a look and see other examples of projects I have undertaken.

# Please Get in Touch!

Either if you are a someone who would like to know more about or simply discuss these topics, or if you are an employer / researcher that would like to collaborate with me, please get in touch! My email is albert.albesa.gonzalez@gmail.com
