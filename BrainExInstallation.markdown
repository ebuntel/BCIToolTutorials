# BrainEx Installation Guide

## Installation Process
The installation process for BrainEx is described below. 

*Note: If you already have Python installed feel free to ignore Step 1.*

### Step 1. Python
BrainEx is a Python library so the first step to using BrainEx is to install Python. BrainEx is written in Python 3.6, but any version 3.6 or later will work. 

Installing Python is as simple as visiting [this](https://www.python.org/downloads/) link, choosing the version of Python you want, and running the executable. 

The versions of Python found on website above come packaged with the pip package manager. We will use this package manager in the next step to install BrainEx's dependecies. 

### Step 2. Install Python Dependencies
BrainEx requires certain Python libraries to be installed before usage. As mentioned above we will use Python's package manager pip to install them. 

```bash
python -m pip install numpy
python -m pip install cython
```

Now, navigate to the "brainex" folder inside of the BrainEx repository. This repo should have a requirements.txt file. If you run the below command in this folder, it will automatically install many of BrainEx's dependencies. 

```bash
python -m pip install -r requirements.txt
```

Finally, run these last commands to install the remaining dependencies. 

```bash
python -m pip install git+git://github.com/ApocalyVec/fastdtw.git
python -m pip install h5py
python -m pip install boto3
```

### Step 3. Run the Setup

The main folder of the BrainEx repository should include a "setup.py" file. This file checks if you have the correct dependencies installed (which we did in Step 2), and installs the BrainEx library itself. 

To run the setup.py file you just have to use the following command:

```
python -m pip install .
```

This should run the setup.py script which will install the BrainEx library on your computer. 

### Step 4. Check the Installation

Now that you've installed the BrainEx library it's best to test if your installation is working correctly. This can be done very easily. 

First, run a Python editor using the python command:

```bash
python
```

This should change your command line to a Python command line allowing you to write Python code in your terminal. To check if BrainEx is correctly installed we can simply attempt to import it:

```python
import brainex
```

If the above command executes without error then BrainEx is correctly installed!

You should now be able to call BrainEx from any python file running on your computer. If you would like more information on how to use BrainEx I would suggest looking at the other tutorials included in this guide. In particular, the BrainEx demo will give you an overview of the system's features. 