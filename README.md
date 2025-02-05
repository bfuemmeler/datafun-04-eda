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

<<<<<<< HEAD
# added all code and tested each one
# added all markdown with observations and insight
# Run All resulted in 0 errors or warnings
=======
2-3-25
Created Markdown title & header
Created Python cell for imports
Created Python cell to load data
>>>>>>> b412eaeca313bcc5743e157f9518a2ab4c561826

# Instructions for EDA below
## Exploratory Data Analysis

Objective: Implement Jupyter Notebook to perform exploratory data analysis
 (EDA) using pandas and other tools. 
We will use the Seaborn library to load the Iris dataset. 
Review the dataset here: iris.csv or see the local copy provided iris.csv.

## Step 1. Initial Title, Header, and Imports
Start by getting organized and providing the focus for your notebook. 
1. Create a single Markdown title. 
2. Create a Markdown header with author name, purpose, and date at the top.
3. Create a numbered section for Imports (using a Markdown cell).
4. Create a Python cell for all the import statements needed for this notebook, for example (yours may vary):

Jupyter Notebook Python cell example:

```python
import pandas as pd
import seaborn as sns
import matplotlib 

# Axes object (basic plot type returned by Seaborn)
from matplotlib.axes import Axes
```

## Step 2. Load Data
Then, we acquire the data and load the data 
into a suitable structure for analysis, 
typically a pandas DataFrame when working with Python. 
Everything we learned about data earlier can be helpful in this step. 
You should be able to read csv, txt, JSON and more.

Some Python tools have datasets built in. 
We'll use these so we can focus on the new skills in this module. 
For example, in this project, we use the Iris dataset available in the Seaborn library. 

The Iris dataset is a well-known dataset in data science and machine learning, 
often used for various classification tasks and basic data exploration.

Load the data into a pandas DataFrame which is used to handle 2-dimensional spreadsheet data.  
We'll use sns.load_dataset() function and pass in the 'iris' (the name without .csv) to populate our DataFrame.

Jupyter Notebook Python cell example:

```python
# Load the Iris dataset into pandas DataFrame
iris_df: pd.DataFrame = sns.load_dataset('iris')

# List column names
iris_df.columns

# Inspect first few rows of the DataFrame
iris_df.head()

```


## Step 3. Initial Data Inspection
Once the data is loaded, the first task is to get a sense of what we're working with.

We can check the first few rows of the dataset using the DataFrame head() method to understand the structure of the data. 
We can pass in an argument with the specific number of rows to view.
We can check the shape of the DataFrame with shape to see the number of rows and columns (an attribute - note there are no parentheses). 
We can see the data types of each column with dtypes (an attribute - note there are no parentheses). 
We can see a bit more by calling the info() method. 
This step is crucial for getting familiar with the dataset's format, size, 
and the type of information each column holds. 

Jupyter Notebook Python cell example:

```python
# Specify the number of rows to display
iris_df.head(10)

# Inspect the shape of the DataFrame with shape attribute
# The shape is a tuple with count of rows and columns in the DataFrame
iris_df.shape

# Inspect the data types of the columns with dtypes attribute
# The data types are returned as a pandas Series
iris_df.dtypes

# Inspect the data types of the columns with info() method
iris_df.info()
```

## Step 4. Initial Descriptive Statistics
The next step is to look at summary statistics.

Use the DataFrame describe() method to obtain a statistical summary of the numerical columns.
This includes count, mean, standard deviation, minimum, and maximum values, as well as the quartiles.
This provides insights into the distribution and central tendencies of the data, which can be crucial for identifying patterns, anomalies, or data integrity issues.

Jupyter Notebook Python cell example:

```python
# Inspect summary statistics for numerical columns
iris_df.describe()
```

## Step 5. Initial Data Distribution for Numerical Columns
We can show a histogram for a single numerical column by providing the EXACT column name. 
To show histograms for ALL numerical columns, we can use hist().

Jupyter Notebook Python cell example:

```python
# Inspect histogram by one numerical column
iris_df['sepal_length'].hist()

# Inspect histograms for ALL numerical columns
iris_df.hist()

# Show all plots
matplotlib.pyplot.show()
```
Afterwards, use a Markdown cell to document your observations.

## Step 5. Initial Data Distribution for Categorical Columns
Choose a categorical column and use iris_df['column_name'].value_counts() to display the count of each category. 
Use a loop to show the value counts for all categorical columns.

Jupyter Notebook Python cell example:

```python
# Inspect value counts by categorical column
# Column name must be EXACT.
# The value_counts() method is only available for Series objects.
# The value_counts() method returns a pandas Series with the counts of unique values in the column.
iris_df['species'].value_counts()

# Inspect value counts for ALL categorical columns
for col in iris_df.select_dtypes(include=['object', 'category']).columns:
    # Display count plot
    sns.countplot(x=col, data=iris_df)
    matplotlib.pyplot.title(f'Distribution of {col}')
    matplotlib.pyplot.show()

# Show all plots
matplotlib.pyplot.show()
```

Afterwards, use a Markdown cell to document your observations.

## Step 6. Initial Data Transformation and Feature Engineering
 Data rarely comes in the format needed for optimal analysis. 
 This phase of data preparation or preprocessing is a multifaceted process that 
 involves both cleaning and transforming the data for analysis. 

The distinction can be subtle, but in general:

***Data Cleaning*** is about ensuring the quality and consistency of the data. This includes:
- Handling missing values to prevent gaps in analysis.
- Removing duplicate entries to avoid skewed results.
- Correcting errors to maintain data accuracy.
- Potentially standardizing formats, such as ensuring dates are consistently formatted or categorical data is uniformly labeled.

**Data Transformation** focuses on preparing the data for analysis. This involves:
- Normalization or standardization of numerical data to bring different scales to a common scale.
- Encoding categorical variables, such as through one-hot encoding, to make them suitable for analysis.
- Renaming columns for clarity and consistency across the dataset.
- Feature engineering, which involves creating new features from existing data.

Use pandas and other tools to perform cleaning and transformations as needed.  
This step refines raw data into a form where additional analytical techniques 
can be applied more effectively.

Jupyter Notebook Python cell example:

```python
# Feature Engineering
# Renaming a column
iris_df.rename(columns={'sepal_length': 'Sepal Length'}, inplace=True)

# Adding a new column
iris_df['Sepal Area'] = iris_df['Sepal Length'] * iris_df['sepal_width']

```

## Step 7. Initial Visualizations
With the data in the right shape, using the features and columns in the desired format, 
the next step is to begin visualization. 
This involves using appropriate chart types to extract and present insights from the data.

Libraries like seaborn and matplotlib offer a wide range of visualization options. 
For instance, pair plots from seaborn can be very useful for understanding relationships between all variables in a dataset. 
Create a variety of chart types using seaborn and matplotlib to showcase different aspects of the data. 

Jupyter Notebook Python cell example:

```python
# Feature Engineering
# Renaming a column
iris_df.rename(columns={'sepal_length': 'Sepal Length'}, inplace=True)

# Adding a new column
iris_df['Sepal Area'] = iris_df['Sepal Length'] * iris_df['sepal_width']

# Create a pairplot of the Iris dataset
# A pairplot is a grid of scatter plots for each pair of numerical columns in the dataset
# The hue parameter is used to color the data points 
# by species (a categorical column)
sns.pairplot(iris_df, hue='species')

# Show all plots
matplotlib.pyplot.show()
```
Important: After each visualization, use Markdown cells to document your observations and insights.

Add a scatter plot - good for showing two numerical variables with a categorical attribute as the color of the dot at each xy point.

Jupyter Notebook Python cell example:

```python
# A scatter plot is a plot of two numerical variables.
scatter_plt: Axes = sns.scatterplot(
    data=iris_df, x="Sepal Length", y="Sepal Area", hue="species"
)

# Set axis labels using the Matplotlib Axes methods set_xlabel() and set_ylabel()
scatter_plt.set_xlabel("Sepal Length (mm)")
scatter_plt.set_ylabel("Sepal Area (mm squared)")   

# Set the title using the Matplotlib Axes set_title() method
scatter_plt.set_title("Chart 1. Iris Sepal Length vs. Sepal Area (by Species)")

matplotlib.pyplot.show()
```

## Step 8. Initial Insights
Use your chart headings and annotations to provide your insights. 
At the end add a section that summarizes your initial insights based on the facts discovered during your initial exploratory data analysis. 

## Step 9. Annotate Your Notebook for Storytelling and Presentation
The final step of the EDA process is interpreting the visualizations and 
statistics to craft a compelling narrative around your findings. 
This involves combining your technical analysis with storytelling techniques to 
make your findings clear and engaging for your audience. 
The goal is to provide actionable insights and convey the significance of your 
findings in a way that resonates with stakeholders, regardless of their 
technical background.

Use your own custom opening to introduce yourself and the focus of your notebook. 
Use Markdown section headings to introduce each step. 
Interpret the visualizations and statistics to narrate a clear and compelling data story. 
Present your findings in a logical and engaging manner.
Present your notebook with an opening that introduces yourself and your topic. 
Use Markdown section headings to introduce each step. 
Interpret the visualizations and statistics to narrate a clear and compelling data story. 
Present your findings in a logical and engaging manner.

## Checklist

- [ ] Notebook has exactly one Markdown title (with a single hash).
- [ ] Notebook has useful Markdown header cell with author and purpose, and optionally, the date.
- [ ] Notebook uses numbered second level Markdown headings for organization. 
- [ ] Notebook has numbered sections with useful content for:
  - [ ] 1. Imports
  - [ ] 2. Load Data
  - [ ] 3. Initial Data Inspection
  - [ ] 4. Initial Descriptive Statistics
  - [ ] 5. Initial Data Distribution for Numerical Columns
  - [ ] 6. Initial Data Transformation and Feature Engineering
  - [ ] 7. Initial Visualizations
  - [ ] 8. Initial Insights
- [ ] Notebook includes commentary as we go that tells a unique data story. 
- [ ] Notebook includes unique insights into the dataset. 
- [ ] Code and visuals are working, notebook is fully executed and on display in GitHub. 