# Analyzing the DTRS Datasets

This set of Jupyter Notebooks is set up to analyze the DTRS datasets.

## Prerequisites
Before starting, though, please check if you have the following
software.
If not, please follow the instructions below to install them.

### Python 3.8
This should work on Python 3.6 or older, but if you do not have Python
installed on your system, you are better off installing version 3.8.
Assuming you are on a Mac, [download this installer here.](https://www.python.org/ftp/python/3.8.6/python-3.8.6-macosx10.9.pkg)
Once the installation is done, open Terminal and type the following
command:

```bash
which python3
```
...and make sure the response has something about 3.8.x.

### Python Package Installer (PIP)

If you installed Python the way above, you should have access to `pip`
directly.
To check, you can type the command

```bash
which pip3
```

#### If you do not have PIP installed
If you find out that `pip` is not installed, you should download the
file `get-pip.py` using the following commands:

```bash
curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
```

Assuming you are still in the same directory, you can then type

```bash
python3 get-pip.py
```
### Python Libraries

We use a number of Python libraries for this work.
Please check if you have them all, or install them using the commands
provided below:

#### Numpy
For numerical computing (matrices/vectors etc.)
```bash
pip3 install numpy
```

#### Pandas
Data manipulation and analysis tool.
```bash
pip3 install pandas
```

#### Seaborn
Plotting library, works well with Pandas.
```bash
pip3 install seaborn
```

#### Spacy
One of the newer and faster NLP libraries.

```bash
pip3 install spacy
```
Download the English language model for Spacy:

```bash
python -m spacy download en_core_web_sm
```

#### Empath
To create custom linguistic categories

```bash
pip3 install empath
```
#### Jupyter
Computational notebook based on Python.
```bash
pip3 install jupyter
```

## This Repository
Now that you have all the installation out of the way, you can clone
this repository, or download it as a zip file (see link on top).

## Datasets
You should already have access to the datasets separately.
Copy the `.txt` files and paste them into the `output` folder.
If the folder does not exist, create it in the top-level folder that
contains the `.ipynb` files (the Jupyter Notebooks).

## Launch the Notebook

If all goes well, you should be able to launch Jupyter using Terminal.
Open Terminal, navigate to the cloned/downloaded directory, and type the
following:

```bash
jupyter notebook
```
Sometimes there may be issues with the shortcuts (some `$PATH` variables
need to be set up), and Jupyter may not launch. If this happens, try
this alternative:

```bash
python3 -m jupyter notebook
```

If all goes well, you should have your default browser automatically
open with the notebook.
If not, open your default browser and type the following into the
address bar:

`localhost:8888/tree`

#### NOTE:
You do not need to run the notebook titled `file_parsing.ipynb`. You
already have the output of that notebook in your `outputs` folder.
You can go to one of the LIWC or Empath notebooks and run them.
