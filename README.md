# Pro Analytics 01: Setup and Workflow Guide

This repository provides a clear, concise guide to help set up a machine for Python projects, 
initialize a new Python project, and follow a repeatable project workflow 
when developing professional Python projects. 

The instructions are divided into three main sections.

## First: Setup Machine and Sign up for GitHub
Go to [01-machine-setup](01-machine-setup/MACHINE-SETUP.md) to prepare for Python projects.
Start here to set up a machine for the first time (or to upgrade or verify professional tools).

This section contains **one-time tasks** including:
1. View file extensions and hidden files and folders.
2. Install (or verify) a package manager for your operating system.
3. Install Python, Git, and Visual Studio (VS) Code for your operating system.
4. Configure Git
5. Install common VS Code extensions.
6. Create a Projects folder to hold your projects. 
7. Create a GitHub account.

---

## 02-Project-Initialization
Go to [02-Project-Initialization](02-Project-Initialization/) when **starting a new project**.

This section walks you through the steps to either:
1. Copy an existing project OR start a new project from scratch.
2. Clone your new GitHub repo to your machine. 
3. Add common files such as .gitignore and requirements.txt.
4. Git add-commit-push the changes to GitHub.
5. Create a local project virtual environment for Python.

---

## 03-Repeatable-Workflow
Go to [03-Repeatable-Workflow](03-Repeatable-Workflow/) for ongoing project development.

This section provides the **repeatable steps** for working on Python projects. 
These steps are typically followed whenever we make changes to a project. The workflow includes:
1. Pull any recent changes from GitHub.
2. Activate the virtual environment.
3. Install dependencies.
4. Run scripts and/or Jupyter notebooks.
5. Make updates, verify the code still runs, and git add-commit-push to GitHub. 

---

## Important

- Follow the instructions carefully.
- Follow the instructions in the recommended order.
- Verify each step before proceeding. 

## Celebrate
Follow each step carefully. 
We have helped hundreds of new analysts get started with professional Python. 
Verify you can run both a script and a notebook successfully. 
Then, celebrate - that's a big iceberg needed to get started with Professional Python.

## Follow The Proven Path Provided
Hopefully, each step is not too bad and things go well. 
When they don't - that's to be expected. 
Part of the reason we get hired is to "figure things out" and we are here to help you do that. 
Learn to do a web search, and experiment with free AI assistants to help explain and provide any additional details needed. 
Remember, YOU are in charge. 
This is the process we support and these instructions work. 
Do NOT deviate unless you agree to invest time and energy to ensure any of the many alternate paths work for you throughout the program. 

## Explore
AFTER that is where the power and joy of working with Python begins. 
Keep good notes. 
Save the working versions and then, change things. 
- Rename a variable. 
- Add a new statement. 
- Comment things out.
- Rename a function. 
- Check out the logs. 

Working with code is a fun, safe, rewarding way to learn. 
If you enjoy puzzles, getting value from Python is a great way to earn a living. 

# Introduction to Jupyter Notebooks in VS Code

Jupyter Notebooks are a popular way to create and share documents for data analytics. 
They are interactive, easy to share, and support a wide variety of data science tools.

When employers ask for years of experience with a language, it's not the syntax - that can be learned in a few days. 
It's the experience with the tools, libraries, and frameworks that takes time.

IMPORTANT: To run Jupyter within VS Code, use the Jupyter extension. Go to the Extensions pane on the left sidebar (the icon looks like four squares), searching for "Jupyter," and installing the "Jupyter" extension provided by Microsoft.

---

## Task 1: Use and Explore the Demo Project / Repository / Notebook

### Step 1: Copy and Clone the Example Repository
1. Click "Use this template" on this example repository (if it's not a template, click "Fork" instead).
2. Clone the repository to your machine:
   git clone example-repo-url
3. Open your new cloned repository in VS Code.

### Step 2: Set Up and Run the Demo Notebook
Next, create and activate a virtual environment for this project. 
Also install additional dependencies required for this project.
See [requirements.txt](requirements.txt) for detailed instructions. 

A. Create .venv
B. Activate .venv
C. Install dependencies into .venv
D. Select VS Code interpreter to use .venv

### Step 3: Open Notebook, Create/Select Kernel
1. Open the provided Jupyter Notebook (`demo-notebook.ipynb`):
2. Create and select the notebook kernel. See [requirements.txt](requirements.txt) **Step E** for detailed instructions. 

### Step 4: Explore the Notebook Cells and Code
Open the Notebook and click Run all to execute it.
- Explore how notebooks have cells. 
- Our notebook cells are either Markdown or Python. 
- Try to add new cells.
- Try to change the type of a cell.
- Try some Markdown in a Markdown cell.
- Try some Python in a Python cell. 
- Review the code and see how it works. 

---

## Troubleshooting and Tips
- See [TROUBLESHOOTING.md](docs/TROUBLESHOOTING.md)

## Additional Resources 
- See [RESOURCES.md](docs/RESOURCES.md)

