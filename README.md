# Description
This is an ML agent that will play Street Fighter 2 using the Gym-Retro library. Hadoukenator is trained with the PPO RL algorithm from OpenAI.

# How to set up your environment
In order to use this agent, some setup is required. These steps are written for using Miniconda.

1. Set up a `conda` virtual environment with python 3.8. Ex: `conda create -n "myenv" python=3.8.0`
2. Activate your environment: `conda activate myenv`
3. With your conda environment active, set your python interpretter in VSCode to your environment.
4. The first time you open the notebook, run the `!pip install gym gym-retro` to get the package in your environment.
5. Bob's your uncle.

# Best parameters
In our hyperparameter tuning, we found these values to be best:
```py
{
    'n_steps': 4160,
    'gamma': 0.9733213457860905,
    'learning_rate': 5e-7,
    'clip_range': 0.12262755315258014,
    'gae_lambda': 0.9318708202044405
}
```