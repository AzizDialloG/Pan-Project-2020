# Pan-Project-2020
# The Project Objective (Problem Statement)
This project concerns the well-known Fisher’s Iris data set [3]. You must research the data set and write documentation and code (in Python [1] to investigate it. An online search for information on the data set will convince you that many people have investigated it previously. You are expected to be able to break this project into several smaller tasks that are easier to solve, and to plug these together after they have been completed. You might do that for this project as follows:
1. Research the data set online and write a summary about it in your README.
2. Download the data set and add it to your repository. 
3. Write a program called analysis.py that: 

	• outputs a summary of each variable to a single text ﬁle,

	• saves a histogram of each variable to png ﬁles, and 

	• outputs a scatter plot of each pair of variables.

## Project Plan

The project plan is to follow the suggestion in the project outline with the combining of some tasks.
My plan for the project is broken down into three areas:
### 1. Research, Document and Summarise Fisher's Iris Dataset
#### Plotting for exploratory data analysis EDA
Exploratory Data Analysis (EDA) is an approach to analyzing datasets to summarize their main characteristics. It is used to understand data, get some context regarding it, understand the variables and the relationships between them, and formulate hypotheses that could be useful when building predictive models. [1]

#### What is EDA?
EDA is a task of analyzing a data using simple tools, from statistics, from plotting tools, from linear algebra, and other techniques.
#### What is Iris data set?
The Flower iris is used by R.A fisher in his research paper in 1936, to use for the multiple classification problem. Dataset is also available on Kaggele and UCI. [2]

The major purpose of this project is to show some graphs i.e. data visualization like histograms and scatter plots. Where Histograms are similar to bar charts shows counts of data in bins and scatter plots show relationship between two data points, one can use third variable for the radius of circle of plot as well.

#### Understanding the IRIS data set:
The total count of data is 150 rows, 50 rows for each class.

There are four features consists on these columns.
	 
	 SepalLength
	 SepalWidth
	 PetalLength
	 PetalWidth
	 Species

#### Those 4 Features are also called as:
Variable/Input-variable/Independent-variable 
And labels (here species) are also called as
 Dependent-variable/out-variable/class/class-label/Response label.
The class variable is "Species". It has 3 number of classes.
#### Classes are below:
	Iris-setosa
	Iris-versicolor
	Iris-virginica

### 2. Download, Code and Summarise
Download the data set and write some code to do the chosen analysis (ie. max, min, mean etc).
MAKE SURE TO ADD COMMENTS TO MY CODE.

#### Libraries that are mandatory for this analysis:

Python | os.listdir() method
os.listdir() method in python is used to get the list of all files and directories in the specified directory. If we don’t specify any directory, then list of files and directories in the current working directory will be returned. [3]


Python | matplotlib. pyplot as plt
pyplot is matplotlib's plotting framework. That specific import line merely imports the module "matplotlib.pyplot" and binds that to the name "plt [4]

Pandas is the most popular data manipulation package in Python, and DataFrames are the Pandas data type for storing tabular 2D data.[5]
CSV (comma-separated value) files are a common file format for transferring and storing data. The ability to read, manipulate, and write data to and from CSV files using Python is a key skill to master for any data scientist or business analysis.[5]

# Load the Pandas libraries with alias 'pd' 
import pandas as pd 
# Load the Pandas libraries with alias 'pd' 
import pandas as pd 
# Read data from file 'filename.csv' 
# (in the same directory that your python process is based)
# Control delimiters, rows, column names with read_csv (see later) 
data = pd.read_csv("filename.csv") 
# Preview the first 5 lines of the loaded data 
data.head(
# Preview the first 5 lines of the loaded data 
data.head()

#### Python | Pandas Series.describe()	
The describe() function is used to generate descriptive statistics that summarize the central tendency, dispersion and shape of a dataset’s distribution, excluding NaN value [6]

#### What Is a Histogram? 
A histogram is a graphical representation that organizes a group of data points into user-specified ranges. It is similar in appearance to a bar graph. The histogram condenses a data series into an easily interpreted visual by taking many data points and grouping them into logical ranges or bins. [7]
_Creating Histograms using Pandas

#### SCATTER PLOT
Scatter Plots (also called scatter diagrams) are used to investigate the possible relationship between two variables that both relate to the same "event." A straight line of best fit (using the least squares method) is often included. [8]

#### _How to Save a Plot to a File Using Matplotlib
The .savefig() method requires a filename be specified as the first argument. This filename can be a full path and as seen above, can also include a particular file extension if desired. If no extension is provided, the configuration value of savefig.format is used instead. [9]
Note that c should not be a single numeric RGB or RGBA sequence because that is indistinguishable from an array of values to be colormapped. If you want to specify the same RGB or RGBA value for all points, use a 2-D array with a single row. Otherwise, value- matching will have precedence in case of a size matching with x and y [10]

### 3. Final Summary
Summarise my findings on the project. Is there any interesting findings? Did I come across someone else's analysis that was interesting? If so, say a little something about it and reference it. Make sure to include why this small data set is popular to analyze.


## References and resources:
#### [1]. https://towardsdatascience.com/how-to-perform-exploratory-data-analysis-with-seaborn97e3413e841d
#### [2]. https://www.kaggle.com/arshid/iris-flower-dataset
##### https://www.neuraldesigner.com/learning/examples/iris-flowers-classification
##### https://www.tutorialspoint.com/python/os_listdir.htm
##### https://matplotlib.org/3.1.1/tutorials/index.html
#### [3]. https://www.geeksforgeeks.org/python-os-listdir-method/
#### [4]. https://matplotlib.org/tutorials/introductory/pyplot.html
#### [5]. https://www.shanelynn.ie/python-pandas-read_csv-load-data-from-csv-files/
##### [How to Import CSV Files to Google's Colab Notebooks]
##### .https://www.youtube.com/watch?v=SHYAQHDQoU4
##### [Google Colab - Executing External Python Files]
##### .https://www.tutorialspoint.com/google_colab/google_colab_executing_external_python_files.htm
##### https://www.datacamp.com/community/tutorials/pandas-read-csv
#### [6] https://www.w3resource.com/pandas/dataframe/dataframe-describe.php
##### http://www.datasciencemadesimple.com/descriptive-summary-statistics-python-pandas/
#### [7] https://www.investopedia.com/terms/h/histogram.asp
##### https://www.datacamp.com/community/tutorials/histograms-matplotlib
##### https://matplotlib.org/api/pyplot_api.html
##### https://www.geeksforgeeks.org/dealing-with-rows-and-columns-in-pandas-dataframe/
##### https://www.programcreek.com/python/example/102365/matplotlib.pyplot.savefig
#### [8] https://www.skymark.com/resources/tools/scatter_plots.asp
#### [9]. https://chartio.com/resources/tutorials/how-to-save-a-plot-to-a-file-using-matplotlib/
##### https://problemsolvingwithpython.com/06-Plotting-with-Matplotlib/06.04-Saving-Plots/
#### [10]. https://matplotlib.org/3.1.1/api/_as_gen/matplotlib.axes.Axes.scatter.html
##### https://matplotlib.org/3.1.3/api/_as_gen/matplotlib.axes.Axes.scatter.html
