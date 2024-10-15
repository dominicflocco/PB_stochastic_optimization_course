# In-Class Activities for Stochastic Optimization Course
Instructors: Steven A. Gabriel, Dominic C. Flocco\
Date: October 2024

This repository contains a set of Jupyter notebooks meant to complement lectures on the Stochastic Optimization as part of the in-person course at Petrobras. The repository contains three notebooks:
* Module 1, Example 1: Two-Stage Recourse Problem - The Farmer's Problem
* Module 1, Example 2: Multi-Stage Recourse Problem - Electricity Market Contracts
* Module 2, Example 1: Risk Measures - Electricity Retailer Problem

The notebooks are designed to be self-contained but coecide with the in-person lectures of the course. The notebooks implement optimization models using [Pyomo](http://www.pyomo.org), a Python-based, open-source optimization modeling language. 

## Getting Started

There are two main options for installing and running the Jupyter notebooks (1) remotely or (2) locally. For users with limited Python programming experience, running the notebooks remotely via [Google Colab](https://colab.research.google.com) is highly recommended. Users comfortable with environment management in Python and command line interfaces may prefer option 2. 

### Running Notebooks in Google Colab (recommended)

Google Colaboratory is a free, browser-based tool that allows users to write and run Python code. To access and run the notebooks on Google Colab, click on the following links: 
* Module 1, Example 1: [module1_example1.ipynb](https://colab.research.google.com/drive/12M7ISAzhnRoAzE0tc8rzz0EA3x_gN9Cc?usp=sharing)
* Module 2, Example 2: [module1_example2.ipynb](https://colab.research.google.com/drive/1fH9Et94IFkfjqeksw_4Q8hUQrgk1M7zK?usp=sharing)
* Module 2, Example 1: [module2_example2.ipynb](https://colab.research.google.com/drive/1-RO5FpAucHQ5xoRY4FVY48a9_HjLtWMV?usp=sharing)

The above links will open the notebooks in a separate web browser. To edit the notebooks, users must save a copy of the notebook to their Google Drive which can be done from the menu `File -> Save a copy in Drive`. The first cell in each notebook will install the necessary package dependecies. Once you run this cell you will be good to go! 

### Running the Notebooks Locally 

To run the notebooks locally, there are two main options: (1) running on a jupyter server or (2) running on VS Code. Both of these steps require cloning this repository via the following command: 

```
git clone https://github.com/dominicflocco/PB_stochastic_optimization_course.git
```
In addition, both methods assume [pip](https://pip.readthedocs.io/en/stable/installing/) and [Anaconda](https://docs.conda.io/projects/conda/en/latest/user-guide/install/index.html) are installed on your local machine. 

#### The Jupyter Server  
The Jupyter notebook is a web-based notebook environment for interactive computing. 

1. First, you will need to create your conda environment using the `toy_env.yml` file:
    ```
    conda env create -f toy_env.yml
    ``` 
    This will create a conda environment on your local machine and install all dependencies needed to run the notebooks. 

2. Then, activate the environment: 
    ```
    conda activate toy_env
    ```
    
3. Once the environment is activated, navigate to the directory of your cloned repository and run the following command to start the Jupyter session: 
    ```
    jupyter notebook
    ```
    This will start a remote connection to the Jupyter server and open this repository in your web browser. Clicking on one of the notebooks will start a new kernel and allow you to run the notebooks.



#### VS Code Set-Up
Alternatively, [Visual Studio Code](https://code.visualstudio.com)  recently introduced support to run Jupyter notebooks natively. To run these notebooks directly in Visual Studio code, perform Steps 1 and 2 above to install and activate your conda environment. Then, open VS Code and follow [these instructions](https://code.visualstudio.com/docs/datascience/jupyter-notebooks) to open and run the notebook in VS Code.



