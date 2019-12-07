[//]: # (Image References)

[image1]: https://video.udacity-data.com/topher/2018/June/5b1ea778_reacher/reacher.gif "Trained Agent"

# Project 2: Continuous Control

### Introduction

In this second project an agent will be trained to move a double-jointed arm to given target locations and to maintain that location.

![Trained Agent][image1]

A reward of +0.1 is provided for each time step that the arm hits the target location. Thus, the goal of the agent is to maintain the arm at the target location for as many time steps as possible.

The state space has 33 dimensions and contains the arm's position, rotation, velocity as well as the arm's angular velocities. Given this information, the agent has to learn how to best generate torque values for all four continuous actions.

The task is episodic, and in order to solve the environment, the agent must get an average score of +30 over 100 consecutive episodes.

### Getting Started

1. If you haven't already, please follow the instructions in the [DRLND GitHub repository](https://github.com/udacity/deep-reinforcement-learning#dependencies) to set up your Python environment. These instructions can be found in README.md at the root of that repository. By following these instructions, you will install PyTorch, the ML-Agents toolkit, and a few more Python packages required to complete the project.

2. Clone this repository.

3. Download the reacher environment from one of the links below. You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)

    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) to obtain the environment.

4. Place the file in this repository and unzip (or decompress) the file.

### Instructions for Starting to Train the Agent

1. Execute `jupyter notebook` on the CLI at the location you put the repository.

2. Click on `Continuous Control.ipynb` in the opened browser window to open the notebook containing the training code.

3. Before running the code and thus actually starting the training the link to the reacher environment needs to be changed to fit the exact path to the above downloaded and unzipped reacher environment.

4. Run the code.

The training will stop after either 1000 episodes or as soon as an average score of +30 is achieved over 100 consecutive episodes. The trained actor and critic models are further stored as `stored_model_actor.pth` and `stored_model_critic.pth` at the repository path.