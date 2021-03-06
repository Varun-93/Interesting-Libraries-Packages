# Interesting-Libraries
> Python Libraries and Packages are a set of useful modules and functions that minimize the use of code in our day to day life. In this article, we are going to discuss some of the interesting libraries and packages.

**NOTE**: Some of these code may not work in **_Python 2_**. Hence I strongly recommend you to try them in **_Python 3_**.

## Table of contents
* [Pillow](#pillow)
* [Howdoi](#howdoi)
* [Wikipedia](#wikipedia)
* [D-Tale](#d-tale)
* [SweetViz](#sweetviz)
* [Vaex](#vaex)
* [Vulture](#vulture)
* [Dataprep](#dataprep)
* [Pyforest](#pyforest)
* [Contact](#contact)


## Pillow
Pillow is a modern version of PIL – Python Image Library. A trusted library while working with images or any type of image format.
It adds image processing capabilities to your Python interpreter.
Features Of Pillow:
* Using Pillow, you can not only open and save images but also influence the environment of images as well.
* Pillow supports a lot of file types such as PDF, WebP, PCX, PNG, JPEG, GIF, PSD, WebP, PCX, GIF, IM, EPS, ICO, BMP, and many others as well.
* Pillow supports a collection of image filters – FIND_EDGES, DETAIL, SMOOTH, BLUR, CONTOUR, SHARPEN, SMOOTH_MORE, and others.

Pillow can be installed using **pip** :

```
$ python3 -m pip install --upgrade pip
$ python3 -m pip install --upgrade Pillow
```

One can find more about this library from here: https://pypi.org/project/Pillow/




## Howdoi
Stuck on a coding problem? Wish to visit StackOverflow without leaving the terminal? With howdoi, you can do it!
It provides instant coding answers via the command line and without opening the browser and read through blogs.

Howdoi answers all sorts of queries:

```
$ howdoi print stack trace python
> import traceback
>
> try:
>     1/0
> except:
>     print '>>> traceback <<<'
>     traceback.print_exc()
>     print '>>> end of traceback <<<'
> traceback.print_exc()
```

Howdoi can be installed using **pip** :

```
$ pip install howdoi
```

One can find more about this library from here: https://pypi.org/project/howdoi/




## Wikipedia
One can use the Wikipedia module to fetch a variety of information from the Wikipedia website.
Search Wikipedia, get article summaries, get data like links and images from a page, and more, this library wraps the official Wikipedia API.

Use the incessant flow of knowledge with Python for daily needs.

```
$ import wikipedia
$ wikipedia.search("Barack")
> [u'Barak (given name)', u'Barack Obama', u'Barack (brandy)', u'Presidency of Barack Obama', u'Family of Barack Obama', u'First inauguration of Barack Obama', u'Barack Obama presidential campaign, 2008', u'Barack Obama, Sr.', u'Barack Obama citizenship conspiracy theories', u'Presidential transition of Barack Obama']
```


Wikipedia can be installed using **pip** :

```
$ pip install wikipedia
```

One can find more about this library from here: https://pypi.org/project/wikipedia/




## D-Tale
The very first step in data science is exploratory data analysis, aka EDA. All types of data models do not fit all data types, so it is better to thoroughly analyze the data before proceeding further.
D-Tale is one of the most interesting libraries to help you tackle your Exploratory Data Analysis(EDA) blues. It is a library that allows us to visualize a Pandas DataFrame.
It generates an interactive graphical interface in which we can define what we want the data to look like and do an exploratory analysis of data as we like.

The good thing about this library is that one can play with the data according to their needs and can not only perform analysis visually but also can extract code to perform that analysis.Dropping NAs, Replacing values, performing required statistics, describing data, finding and plotting correlations all of it can be done in a matter of time.

The only thing that is a pre-requisite is the knowledge of What EDA is and why is it done.
If one is familiar about the term EDA, one can make efficient use of this library and easily perform the analysis. 

D-Tale can be installed using **pip** :

```
$ pip install dtale
```

One can find more about this library from here: https://pypi.org/project/dtale/




## SweetViz
Yet another amazing library to automate the process of EDA and as the name suggests making EDA more sweeter.
An open-source Python library that generates beautiful, high-density visualizations to kickstart EDA with just two lines of code.

It integrates associations for numerical (Pearson's correlation), categorical (uncertainty coefficient) and categorical-numerical (correlation ratio) datatypes seamlessly, to provide maximum information for all data types. Also provide a summarized information on the type, miising and NA values etc.

In addition to creating insightful and beautiful visualizations, it provides analysis such as:
* Comparison of 2 datasets (e.g. Train vs Test)
* Visualization of the target value against all other variables (e.g. “What was the survival rate of male vs female” etc.)

SweetViz can be installed using **pip** :

```
$ pip install sweetviz
```

One can find more about this library from here: https://pypi.org/project/sweetviz/




## Vaex
Some datasets are too large to fit into the main memory of your desktop computer, let alone your laptop. Still, we would like to work with large datasets in the era of Big Data.
Wouldn’t it be great if you could load a 1 Terabyte data file instantly, reading only the parts you need.

Pandas is one of the most used python libraries but it has certain drawbacks like it uses a slow function which is not very suitable for bigger datasets, also pandas only handle results that fit in the memory which can be easily filled.

To overcome these drawbacks of Pandas, we have a high-performance python library for lazy Out-of-Core Dataframes named Vaex which is used to visualize and manipulate big tabular datasets.It makes working with large datasets a breeze. Vaex uses memory mapping, zero memory copy policy and lazy computations for best performance. It never touches or copies the data unless explicitly requested. This makes it possible to work with datasets that are the size of our hard drive.

Vaex can be installed using **pip** :

```
$ pip install vaex
```

One can find more about this library from here: https://pypi.org/project/vaex/




## Vulture
Maintaining a high level of code quality is important for any serious project. One aspect of this is ensuring that all code is actually used. There are many reasons for dead code ending up in a project. The most common is refactoring, but another is misspellings, which are only detected at runtime for dynamic languages. Finding and removing dead code allows to keep the code base clean and reduces bugs.

As the name suggests, Vulture finds dead code or code which is unused in Python programs. This is useful for cleaning up and finding errors in large code bases.

The only drawback of this library is the false positives are common. But it can be handled too with some tweaks. 

After installation, it is simple to use:
```
$ vulture path/to/code
```
For example, given this small bit of Python:
![Vulture1 screenshot](./img/Vulture/vulture1.PNG)

Saving that and running vulture against it will give us the following output:
![Vulture2 screenshot](./img/Vulture/vulture2.PNG)

It cleverly finds the variable defined in a function that isn't used. It does know that the function is used.

Vulture can be installed using **pip** :

```
$ pip install vulture
```

One can find more about this library from here: https://pypi.org/project/vulture/




## Dataprep
Dataprep is another open-source python library that allows you to prepare your data and that too with just a few lines of code.
There are various things that can be performed with the help of Dataprep:
* Collect data from common data sources(dataprep.connector). Connector provides a simple wrapper to collect structured data from different Web APIs (e.g., Twitter API, Spotify API), making web data collection easy and efficient, without requiring advanced programming skills.
* Perform exploratory data analysis(dataprep.eda).
* Clean and standardize data(dataprep.clean) by providing a large number of functions with a unified interface for cleaning and standardizing data of various semantic types in a Pandas DataFrame. For example, clean_email() function supports cleaning of messy email values by doing the strict semantic type check.

![Dataprep screenshot](./img/dataprep/dataprep.PNG)

Dataprep can be installed using **pip** :

```
$ pip install dataprep
```

One can find more about this library from here: https://pypi.org/project/dataprep/




## Pyforest
Sometimes, it happens that we spent a huge amount of time importing some common libraries like NumPy, pandas, matplotlib, seaborn, nltk and many more. To remove this headache of importing such libraries manually, we have pyforest library.
Pyforest lazy-imports all popular Python Data Science libraries so that they are always there when you need them. If you don't use a library, it won't be imported.

Types of functions used in pyforest are:
* **lazy_imports():** Returns all the libraries available in pyforest.
* **active_imports():** Returns all the libraries which have been used in the program.
 
The advantage of using this library can be observed from the following:
* **Without Pyforest:**
![Dataprep screenshot](./img/pyforest/without.PNG)

* **With Pyforest:**
![Dataprep screenshot](./img/pyforest/with.PNG)

All of these & more can be imported using just **_one single line_**

Pyforest can be installed using **pip** :

```
$ pip install pyforest
```

One can find more about this library from here: https://pypi.org/project/pyforest/




## Contact
Created by [@Varun-93](https://github.com/Varun-93) - also feel free to contact me @
[![Linkedin Badge](https://img.shields.io/badge/-VarunBhatia-blue?style=flat-square&logo=Linkedin&logoColor=white&link=https://www.linkedin.com/in/varun-bhatia-a20729a8/)](https://www.linkedin.com/in/varun-bhatia-a20729a8/)

