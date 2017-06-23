# Week 1: Introduction to Machine Learning

In Week 1, we focus on introducing machine learning, the general machine learning workflow, and various tools and techniques (data scraping, exploratory visualization, etc) that we need in the process.

We introduce the various component independently first to put focus on them (with an eye towards how they tie back with general tasks in machine learning).

## Day 1: Introduction

Pre-class Activity
* Set up a `Twitter` account, get the tokens, setup the tokens
* Set up a `GitHub` account, get the token, setup the token
* Get `YAML` data file from Cricsheet.com (to be pre-done in IDE?)
* Complete pre-reading tasks
    - REST API link 1
    - REST API link 2
    - DOM link 1 (scraping perspective)
    - DOM link 2 (scraping perspective)
    - HTML link 1
    - XML link 1
    - JSON link 1
    - YAML link 1
    - CRISP-DM link
---
[15 mins] Pre-class Session
* [5 mins] Overview of the Week
* [5 mins] Overview of the Day
* [5 mins] Flash Quiz
---
Hour 1: DataScience and MachineLearning
* [10 mins] What is Machine Learning? Why do we do Machine Learning? Tom Mitchell's definition
* [5 mins] Supervised vs Unsupervised Machine Learning
    - Examples
* [10 mins] Data Science vs Machine Learning: How do they fit-in with each other?
* [35 mins] How to tackle a real-life Data Science problem (case-study)
    - [15 mins] An example walk-through
    - [5 mins] Where do frameworks like `CRISP-DM` come in?
    - [15 mins] Group discussion with another example
---
Hour 2: Thinking about data for Machine Learning
* [15 mins]
    - Big vs Small
    - Fast vs Slow
    - [5 mins] Offline vs Online Learning
        * With example
    - [5 mins] features and records (p>>n vs n>>p)
    - [5 mins] Blackbox vs Interpretable
* [45 mins] Where does data come from?
    - [5 mins] RDBMS and Datamarts
    - [15 mins] What is NoSQL?
        * Why NoSQL?
        * Vertical vs Horizontal Sharding (scaling)
        * Object-Relational impedance mismatch [Note: We focus on this to motivate real use-cases for NoSQL in Data Science work]
        * Shortcoming - aggregation patterns
    - [15 mins] Where does NoSQL come from?
        * RDBMS Database
        * JSON and YAML
        * Log files on disk
        * [10 mins] APIs and (web) apps
            - REST
            - Graph
            - There is no REST
    - [10 mins] RDBMS vs NoSQL in practice
        * What does it mean for you as a data scientist?
        * Typical use cases
---
Hour 3: Data from the web 1 (Scraping and Parsing)
* [10 mins] Introduction to HTML, DOM, XML
* [10 mins] Scraping websites with `Scrapy`
* [10 mins] Scrapy example:
* [10 mins] Parsing html with `BeautifulSoup4` (BS4)
* [10 mins] BS4 example:
* [10 mins] Summary (combining above examples to parse a csv)
---
Hour 4: Getting the data from the web 2 (APIs and Parsing)
* [15 mins] Querying the GitHub (GH) REST API
    - Question 1
    - Question 2
* [15 mins] Querying the Twitter REST API
    - Question 1
    - Question 2
* [15 mins] Parsing API responses
    - CSV responses
    - JSON responses
    - Example of questions that GH/Twitter APIs can't answer (aggregation)
    - Answering aggregations questions with Python
* [15 mins] Worked out example
    - Reading YAML files into Python
    - Converting YAML/JSON imports to CSVs (why? no strong aggregation patterns)
    - A class to read `Cricsheet` YAMLs and produce CSVs
---
Hands-on Session (4 hours)
* New Scraping tasks (`Scrapy`)
* New Parsing tasks (`BeautifulSoup4`)
* Further questions on GH/Twitter APIs (aggregation questions)
* New questions on `Meetup.com` API/ `Reddit` API
* Full implementation of `Cricsheet` parsing as a Python package



## Day 2:

Pre-class Activity
* ???
* Complete pre-reading tasks
    - `matplotlib` link 1
    - `matplotlib` link 2
    - Faceting link 1
    - Faceting link 2
---
[10 mins] Pre-class Session
* [5 mins] Overview of the Day
* [5 mins] Flash Quiz
---
Hour 1: Introduction to exploratory visualization
* [10 mins] What is exploratory visualization and why do we do it?
* [10 mins] Types/Scales of data
    - Nominal
    - Ordinal
    - Interval
    - Ratio
    - These types mostly match up their pd.Series counterparts, but not always
* [20 mins] Basics of `matplotlib`
* [20 mins] Example plots
    - Ask what kind of plot would be appropriate for a dataset/feature to motivate a plot
    - [5 mins] Bar Charts
    - [5 mins] Stacked Bar Charts (and where they are appropriate)
    - [5 mins] Grouped Bar Charts (and where they are appropriate)
    - [5 mins] Scatter Plots
* A bit on Grammar of Plots and why we are not doing Seaborne or Bokeh

---
Hour 2: Being a Data Detective
* [20 mins] Understanding Univariate Data
    - Numeric vs Categorical
    - [5 mins] Histograms
    - [5 mins] Q-Q Plots
    - [5 mins] Box and Whiskers Plots
    - [5 mins] Visualizing missing data
* [20 mins] Understanding Bivariate Data
    - [5 mins] Numeric vs Numeric
        * Scatter Plots
    - [5 mins] Numeric vs Categorical
    - [5 mins] Categorical vs Categorical
    - [5 mins] Correllograms
* [20 mins] Faceting
    - Introduction
    - Reproduce the example from *the lattice book*
---
Hour 3: Transforming and Encoding Data
[Note: Even though we'll be using `sklearn`, the machine learning part of it will not be touched upon. Even though students get comfortable with using the api for machine learning, they often struggle with data processing. The idea is to introduce the general organizational principles behind `sklearn` api before introducing usage.]
* [20 mins] Encoding Categorical variables
    - Why we encode categorical variables
    - Different kinds of encoding
        * Label encoding
        * One-hot encoding
    - Which is the best way to encode categorical variables?
        * Invoke the No Free Lunch Theorem
        * Stress on the empirical nature of machine learning (we'll use this later to motivate (cross) validation)
        * The challenge of learning feature representation
* [20 mins] Introduction to sklearn api
---
Post-class Activities
* Complete post-reading tasks
    - [7 Different categorical variable encoding schemes](http://www.willmcginnis.com/2015/11/29/beyond-one-hot-an-exploration-of-categorical-variables/)
    - [More on encoding categorical variables](https://www.analyticsvidhya.com/blog/2015/11/easy-methods-deal-categorical-variables-predictive-modeling/)
    - [Encoding variables with Pandas and sklearn](http://fastml.com/converting-categorical-data-into-numbers-with-pandas-and-scikit-learn/)
