# A Brief Guide to Jupyter Notebooks

Jupyter Notebook is a commonly used data-science tool that allows its users to run their Python scripts as they're writing them. Jupyter Notebooks consist of chunks of Python code that can be executed independently and each give their own output. This is very convenient for making interactive tutorials so I have written some of the tutorials in this repository as Jupyter notebooks. For those of you who are unfamiliar with Jupyter Notebook, here is a quick guide as well as some useful links. 

## Installation

The easiest way to install Jupyter Notebook is to install [Anaconda](https://docs.anaconda.com/anaconda/install/). If you already installed Anaconda as a part of installing BrainEx then you can skip the rest of this step. 

If you have installed Python without Anaconda, then use the following terminal command to install Jupyter notebook: 
```bash
pip install notebook
```

## Using Jupyter Notebooks

Jupyter Notebook has the same starting command on Linux, Windows, and Mac OSs:

```bash
jupyter notebook
```

The above command starts a Jupyter Notebook server. To access your server simply put the link printed when you started the server into any browser. Yours will look somewhat different but here is an example link:

* http://localhost:8888/?token=a1c2065e7cde2991015bf5900ffa0c8a4e1d95eb9fe3464e

When you are done with your server you can shut it down by terminating the process from the terminal you used to start it. 