# NAML Installation + Usage Tutorial

## Installation Process
The installation process for NAML is described below. 

*Note: If you already have Python installed feel free to ignore Step 1.*

### Step 1. Python

BrainEx is written in Python 3.7, but almost any Python version 3.6 or later will work. 

Installing Python is as simple as visiting [this](https://www.python.org/downloads/) link, choosing the version of Python you want, and running the executable. 

The versions of Python found on website above come packaged with the pip package manager. We will use this package manager in the next step to install NAML's dependecies. 

### Step 2. Dependencies 

The NAML repository comes packaged with a requirements.txt file. This file, conveniently, can be read by Python's package manager to automatically install NAML's required libraries. To do this, simply navigate to NAML's main folder (which contains the requirements.txt file), and run the following command:

'''bash
python -m pip install .
'''