

# Reinforcement Learning project: Navigation

## Introduction


In this project, a model (Agent) was trained to navigate (and collect bananas!) in a large, square world.

![Image of the enviroment](banana.gif)

The enviroment used was *Unity Machine Learning Agents (UMLA)*, where *UMLA* is an open-source Unity plugin that enables games and simulations to serve as environments for training intelligent agents.

 The rules of the enviroment were as follows:

A reward of +1 is provided for collecting a **yellow** banana, and a reward of -1 is provided for collecting a **blue** banana. Thus, the goal of your agent is to collect as many yellow bananas as possible while avoiding blue bananas.

The state space has 37 dimensions and contains the agent's velocity, along with ray-based perception of objects around agent's forward direction. Given this information, the agent has to learn how to best select actions. Four discrete actions are available, corresponding to:

* <span style="padding: .2em .4em; background-color:gray">0</span> - move forward.
* <span style="padding: .2em .4em; background-color:gray">1</span> - move backward.
* <span style="padding: .2em .4em; background-color:gray">2</span> - turn left.
* <span style="padding: .2em .4em; background-color:gray">3</span> - turn right.


On the other hand the model was developed using Pytorch, and the architecture of the model consists of four layers, and batch normalization. 

The model developed avereged a score of 13 over 523 episodes of training! (1000 timesteps per episode in our case)


## Getting started

In order to run the model, we need to set the enviroment first:

1. Download the environment from one of the links below. You need only select the environment that matches your operating system:
    * Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux.zip)
    * Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana.app.zip)
    * Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86.zip)
    * Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Windows_x86_64.zip)

    *(For Windows users)* Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    *(For AWS)* If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P1/Banana/Banana_Linux_NoVis.zip) to obtain the environment.
1. Place the file in the *same folder of this repository* (after you clone it or downlowd it), and unzip (or decompress) the file. 

## Running the agent

> In order to run the agent, you should run <span style="padding: .05em .15em; background-color:gray">Navigation.ipynb</span> with commenting the training cell, unless you want to train your own model.