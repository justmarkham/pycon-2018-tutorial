# Using pandas for Better (and Worse) Data Science

This tutorial was presented by [Kevin Markham](http://www.dataschool.io/about/) at PyCon on May 10, 2018.

## Jupyter notebook

The tutorial code is available as a [Jupyter notebook](tutorial.ipynb). The notebook includes 4 additional exercises that were not covered during the tutorial.

## Video

The [unedited 3-hour tutorial video](https://www.youtube.com/watch?v=0hsKLYfyQZc) has already been posted on the PyCon 2018 YouTube channel. However, about **half of the video is silent**, because that is when students were working on each exercise.

However, I will be **editing the video to remove the silent parts** and releasing it on the [Data School YouTube channel](https://youtube.com/dataschool). To be notified when the edited video is available, please [subscribe to the Data School email newsletter](http://www.dataschool.io/subscribe/).

## What is the tutorial about?

The pandas library is a powerful tool for multiple phases of the data science workflow, including data cleaning, visualization, and exploratory data analysis. However, proper data science requires careful coding, and pandas will not stop you from creating misleading plots, drawing incorrect conclusions, ignoring relevant data, including misleading data, or executing incorrect calculations.

In this tutorial, you'll perform a variety of data science tasks on a handful of real-world datasets using pandas. With each task, you'll learn how to avoid either a pandas pitfall or a data science pitfall. By the end of the tutorial, you'll be more confident that you're using pandas for good rather than evil!

## How well do I need to know pandas to participate?

You will get the most out of this tutorial if you are an intermediate pandas user, since the tutorial will not cover pandas basics. If you are new to pandas or just need a refresher, I recommend watching some videos from my free [pandas course](http://www.dataschool.io/easier-data-analysis-with-pandas/). Alternatively, you can review all of the code from my pandas course in this [Jupyter notebook](http://nbviewer.jupyter.org/github/justmarkham/pandas-videos/blob/master/pandas.ipynb).

## What datasets are we using?

* `police.csv` is the Rhode Island dataset from the [Stanford Open Policing Project](https://openpolicing.stanford.edu/), made available under the [Open Data Commons Attribution License](https://opendatacommons.org/licenses/by/summary/).
* `ted.csv` is the TED Talks dataset from [Kaggle Datasets](https://www.kaggle.com/rounakbanik/ted-talks), made available under the [CC BY-NC-SA 4.0 license](https://creativecommons.org/licenses/by-nc-sa/4.0/).

## How do I download the files from GitHub?

Here are three options that will work equally well:

- If you know how to use git, you can click the green button above and **clone the repository**.
- If you know how to open a ZIP file, you can click the green button above and **download the repository**.
- If you want to download the files individually, **right click on these links** and select "Save As": [`police.csv`](https://raw.githubusercontent.com/justmarkham/pycon-2018-tutorial/master/police.csv), [`ted.csv`](https://raw.githubusercontent.com/justmarkham/pycon-2018-tutorial/master/ted.csv), [`tutorial.ipynb`](https://raw.githubusercontent.com/justmarkham/pycon-2018-tutorial/master/tutorial.ipynb).

## How can I check that pandas and matplotlib are properly installed?

1. Move the CSV files into your working directory. (This is usually the directory where you create Python scripts or notebooks.)
2. Open the Python environment of your choice.
3. If you're using **Jupyter notebook**, run the following code:

    ```python
    import pandas as pd
	import matplotlib.pyplot as plt
	%matplotlib inline
	ri = pd.read_csv('police.csv')
	ted = pd.read_csv('ted.csv')
	ri.driver_age.plot()
	```

4. If you're using **any other Python environment**, run the following code:

    ```python
    import pandas as pd
	import matplotlib.pyplot as plt
	ri = pd.read_csv('police.csv')
	ted = pd.read_csv('ted.csv')
	ri.driver_age.plot()
	plt.show()
	```

If you don't get any error messages, and a plot appears on your screen, then it's very likely that pandas and matplotlib are installed correctly.

## Who is the instructor?

Kevin Markham is the founder of [Data School](http://www.dataschool.io/), an online school for learning data science with Python. He is passionate about teaching data science to people who are new to the field, regardless of their educational and professional backgrounds. Previously, Kevin was the lead data science instructor for General Assembly in Washington, DC. Currently, he teaches machine learning and data analysis to over 10,000 students each month through the Data School [YouTube channel](https://www.youtube.com/dataschool). He has a degree in Computer Engineering from Vanderbilt University and lives in Asheville, North Carolina with his wife and son.

## Can I contact the instructor with questions?

Sure! You can email [kevin@dataschool.io](mailto:kevin@dataschool.io).
