# Getting Started

This project uses [Poetry](https://python-poetry.org/) for dependency management. Please read the [Basic Usage](https://python-poetry.org/docs/basic-usage/) guide to get started (or simply follow the steps below).

```
# Install Poetry
pip install poetry==1.7.1

# Create a virtual environment and install 
# packages in the poetry.lock file
poetry install
```

Note that I am using Python 3.11. If you manage your Python with virtual environments, Poetry will use your active Python instance. If you aren't familiar with virtual environments, a quick start looks like:

```
# Ensure you have pyenv
pip install pyenv

 # Installs Python 3.11 and adds it your path
pyenv install 3.11
```

# Using Stable Baselines

This project has [Stable Baselines3](https://stable-baselines3.readthedocs.io/en/master/guide/quickstart.html) and [RL Zoo3](https://rl-baselines3-zoo.readthedocs.io/en/master/). You can follow either of those guides to begin experimenting with the environment. 

# Environments

Right now, the repo only has access to a Cessna 172P model. The instructions on the [JSBGym repo](https://github.com/sryu1/jsbgym/tree/main) allow you to download more models (including our desired F16 model) and visualization tools. I am currently working to add that to the development container in this project.

To start playing around, I recommend using the following environment:

```
env = gym.make("C172-HeadingControlTask-Shaping.STANDARD-NoFG-v0", render_mode="human")
```