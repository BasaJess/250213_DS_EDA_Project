[![Shipping files](https://github.com/neuefische/ds-eda-project-template/actions/workflows/workflow-03.yml/badge.svg?branch=main&event=workflow_dispatch)](https://github.com/neuefische/ds-eda-project-template/actions/workflows/workflow-03.yml)
# Project - EDA Exploratory Data Analysis

This project is centered around exploratory data
analysis techniques and presentation of results to a client


## House Sales in King County, USA
This dataset contains house sale prices for King County, which includes Seattle. It includes homes sold between May 2014 and May 2015

### Deliverables
This is the list of deliverables"

* This Repo, copied from [template](https://github.com/neuefische/ds-eda-project-template)
* 3 documented Jupyter Notebooks, their contents are described in the structure section below.
* This document, an updated and Organized "Readme"file
* A power point presentation for non-technical clients,wich transcript, pptx and pdf copies are in this repo

### Repo Structure
This repo contains:
* This root folder with 3 Jupyter Notebooks and the assignment description files:
 1. Fetching the data
 2. Cleaning the data
 3. EDA analysis of the data and creation of presentation graphics
* A folder containing the data
* A folder containing the presentation files 

### Presentation Documents
* Housing Market.pptx : a Powerpoint file too large for GitHub. Available upon request, the size is 38.3 M
* Housing Market.pdf: A copy of the pptx file in pdf format
* Transcript.docx: A word cocument containing the Transcrip of the presentation

## Requirements

- pyenv
- python==3.11.3

## Setup

One of the first steps when starting any data science project is to create a virtual environment. For this project I created this environment from scratch. The general workflow consists of... 

* setting the python version locally to 3.11.3
* creating a virtual environment using the `venv` module
* activating your newly created environment 
* upgrading `pip` (This step is not absolutely necessary, but will save you trouble when installing some packages.)
* installing the required packages via `pip`

At the end, you want to make sure that people who are interested in your project can create an identical environment on their own computer in order to be able to run your code without running into errors. Therefore you can create a `requirements file` and add it to your repository. You can create such a file by running the following command: 

```bash
pip freeze > requirements.txt
```

*Note: In rare case such a requirements file created with `pip freeze` might not ensure that another (especially M1 chip) user can install and execute it properly. This can happen if libraries need to be compiled (e.g. SciPy). Then it also depends on environment variables and the actual system libraries.*

### Unit testing (Optional)

If you write python scripts for your data processing methods, you can also write unit tests. In order to run the tests execute in terminal:

```bash
pytest
```

This command will execute all the functions in your project that start with the word **test**.

## Set up your Environment
This repo contains a requirements.txt file with a list of all the packages and dependencies you will need.

Before you can start with plotly in Jupyter Lab you have to install node.js (if you haven't done it before).
- Check **Node version**  by run the following commands:
    ```sh
    node -v
    ```
    If you haven't installed it yet, begin at `step_1`. Otherwise, proceed to `step_2`.


### **`macOS`** type the following commands : 


- `Step_1:` Update Homebrew and install Node by following commands:
    ```sh
    brew update
    brew install node
    ```

- `Step_2:` Install the virtual environment and the required packages by following commands:

    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/bin/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```
### **`WindowsOS`** type the following commands :


- `Step_1:` Update Chocolatey and install Node by following commands:
    ```sh
    choco upgrade chocolatey
    choco install nodejs
    ```

- `Step_2:` Install the virtual environment and the required packages by following commands.

   For `PowerShell` CLI :

    ```PowerShell
    pyenv local 3.11.3
    python -m venv .venv
    .venv\Scripts\Activate.ps1
    pip install --upgrade pip
    pip install -r requirements.txt
    ```

    For `Git-Bash` CLI :
  
    ```BASH
    pyenv local 3.11.3
    python -m venv .venv
    source .venv/Scripts/activate
    pip install --upgrade pip
    pip install -r requirements.txt
    ```
 

 **`Note:`**
    If you encounter an error when trying to run `pip install --upgrade pip`, try using the following command:

   ```Bash
   python.exe -m pip install --upgrade pip
   ```
