# Deep reinforcement learning for controlling a double-jointed arm


## Introduction 
This is the second project of Udacity-Deep Reinforcement Learning Course. The main goal is to create an agent that can control a double-jointed arm to keep in desired locations.

Trained Double-jointed Arms
:-------------------------:
 ![](smart.gif)


The each arm has 33-dimensional representations and a 4-dimensional action. This representation(state) contains information of an agent such as velocity,rotation,  and ray-based perception of the agent.


### Termination Criteria

The task is episodic. That means an agent should obtain an average score of +13 over 100 consecutive episodes.

## Let's go!
At first, we should set up out python environment via following the instructions in [here](https://github.com/udacity/deep-reinforcement-learning#dependencies)

Secondly, we should obtain the environment. You do not have to install Unity but the Reacher environment. Please download and extract the appropriate version, then place it in the path of the Jupyter notebook. There are 2 versions of the environment. Note that we used the second one which has 20 agents on the platform.

   - **_Version 1: One (1) Agent_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Windows_x86_64.zip)

   - **_Version 2: Twenty (20) Agents_**
        - Linux: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux.zip)
        - Mac OSX: [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher.app.zip)
        - Windows (32-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86.zip)
        - Windows (64-bit): [click here](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Windows_x86_64.zip)
    
   - (_For Windows users_) Check out [this link](https://support.microsoft.com/en-us/help/827218/how-to-determine-whether-a-computer-is-running-a-32-bit-version-or-64) if you need help with determining if your computer is running a 32-bit version or 64-bit version of the Windows operating system.

   - (_For AWS_) If you'd like to train the agent on AWS (and have not [enabled a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md)), then please use [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/one_agent/Reacher_Linux_NoVis.zip) (version 1) or [this link](https://s3-us-west-1.amazonaws.com/udacity-drlnd/P2/Reacher/Reacher_Linux_NoVis.zip) (version 2) to obtain the "headless" version of the environment.  You will **not** be able to watch the agent without enabling a virtual screen, but you will be able to train the agent.  (_To watch the agent, you should follow the instructions to [enable a virtual screen](https://github.com/Unity-Technologies/ml-agents/blob/master/docs/Training-on-Amazon-Web-Service.md), and then download the environment for the **Linux** operating system above._)


  - Open the notebook named Continuous_Control.ipynb
  - In the second cell, you should write your path for Reacher environment that we mentioned above. 
  - Then you may execute each cell orderly.
  - After the seciton 4, our ml-agent is trained. If you want to use pre-trained weights, follow the below instructions.

## Using a pretrained version
If you are impatient, then you may use the pre-trained model parameters in the repository named checkpoint.pt. All you need to do is to set USE_PRETRAIN variable to True. This variable can be found in the beginning of the 4th section in Continuous_Control.ipynb notebook.
  
  
If you are struggle to work on this project, please just open an issue. Look forward to hear about your nice experiences!
