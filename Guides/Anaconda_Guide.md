# How to Use Anaconda

## Installation

Install Anaconda:
https://www.anaconda.com/download

Guide:
https://www.youtube.com/watch?v=UTqOXwAi1pE 

## Environment Management

Once Anaconda is installed, you can create new environments for different projects. Environments allow you to isolate dependencies and packages.

### Creating a New Environment

#### Using Anaconda Navigator:
1. Open Anaconda Navigator from your start menu or terminal.
2. Click on the "Environments" tab on the left sidebar.
3. Click the "Create" button.
4. Enter a name for your new environment and choose the Python version.
5. Select the packages you want to install in this environment.
6. Click the "Create" button to create the environment.

#### Using the Command Line:
Open a terminal or command prompt and use the following command to create a new environment:
`conda create --name myenv python=3.x`

Replace myenv with your desired environment name and 3.x with the Python version you want.

### Activating and Deactiving Environments

After creating an environment, you need to activate it before using it.

#### Activating an Environment

##### Using Anaconda Navigator:
1. In Anaconda Navigator, go to the "Environments" tab.
2. Click on the environment you want to activate.
3. Click the "Play" button to activate it.

##### Using the Command Line:
`conda activate myenv`

#### Deactivating an Environment
To deactivate the current environment and return to the base Anaconda environment, use the following command:
`conda deactivate`

## Installing Packages

You can install packages within your active environment using the conda install command. For example:
`conda install numpy`

This will install the NumPy package in the active environment.

## Removing an Environment

If you no longer need an environment, you can remove it.

### Using Anaconda Navigator:

1. In Anaconda Navigator, go to the "Environments" tab.
2. Select the environment you want to remove.
3. Click the "Remove" button.

### Using the Command Line:
`conda remove --name myenv --all`

Replace `myenv` with the name of the environment you want to remove.