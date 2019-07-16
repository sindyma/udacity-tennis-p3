
# udacity-tennis-p3
Solving a variation of the Unity tennis environment using deep reinforcement learning. This repo contains a project to meet requirements for the Udacity Reinforcement Learning Nanodegree.

# Background
This is the first project in [Udacity's Deep RL nanodegree](https://www.udacity.com/course/deep-reinforcement-learning-nanodegree--nd893). In this project we work with the [Tennis](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Learning-Environment-Examples.md#tennis) environment. 

In this environment, two agents control rackets to bounce a ball over a net. If an agent hits the ball over the net, it receives a reward of +0.1.  If an agent lets a ball hit the ground or hits the ball out of bounds, it receives a reward of -0.01.  Thus, the goal of each agent is to keep the ball in play.

The observation space consists of 8 variables corresponding to the position and velocity of the ball and racket. Each agent receives its own, local observation.  Two continuous actions are available, corresponding to movement toward (or away from) the net, and jumping. 

The environment is solved when the agent achieves an average score of +0.5 (over 100 consecutive episodes, after taking the maximum over both agents).

### Getting Started

1. Download the environment from one of the links below.  You need only select the environment that matches your operating system:
    - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux.zip)
    - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis.app.zip)
    - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86.zip)
    - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Windows_x86_64.zip)
    
    (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

    (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P3/Tennis/Tennis_Linux_NoVis.zip) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)

2. Clone this repo and place the file in the cloned folder, and unzip (or decompress) the file. 

```git clone https://github.com/sindyma/udacity-tennis-p3.git```

Before running the Jupyter Notebook, ensure all requirements are installed. To do this, navigate to the cloned repo and run the following command. This will install all packages specified in `requirements.txt`.

```pip install .```

Open Navigation.ipynb in the root directory. This Jupyter Notebook trains an RL agent to navigate the environment and collect bananas.

# Troubleshooting
If you aren't able to get started, see if any of the following describe your situation:
* Python version
This repo has been developed with python 3.7. Python 2 users may need to switch their kernel and ensure all dependencies have been installed for python 3.7
* Dependencies
You may need to install dependencies:
* unity-ml
* numpy
* torch
* matplotlib

# Train an agent
Run all the cells in `Tennis.ipynb` to train your own agent. At the end of training, your weights will be saved in the folder as `<dateandtime>_trained_agent.pth`.

# Run a trained agent
The final section in `Tennis.ipynb` runs a trained agent (submission for the project).

