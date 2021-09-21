Preface
=======

Preface from the Second Edition
-------------------------------

by Jan Pearce and Jacqueline Boggs

We are excited to bring you this enhanced version of this book.
As we were planning to teach a course in data analytics,
a course which is cross listed in computer science and business at our institution,
we found it quite challenging to identify a book that had appropriate content
for this type of interdisciplinary course. We were so very excited to find this
open source book due to the clear focus on the data.
We both believe that curiosity is exactly what drives data science and data analytics.
When we encounter a set of data, it leads us to ask provocative questions that
can often be answered by the data techniques covered in this book.

As professors, we believe it is crucially important that students build
life-long learning skills. We have found that it is sometimes difficult for students
to transfer learning to another area/topic/dataset.
For these reasons, we wanted to add some additional datasets into this book,
so we could help students learn to better apply and transfer their knowledge.

Some of the key changes from the First Edition include:

* Learning Goals, Learning Objectives, and Glossaries added to each chapter.
* Chapter titles that identify the data technique to be utilized while still letting curiosity about each of the datasets drive the exploration.
* The fourth chapter has been significantly expanded to include a targetted introduction/review of Python.
* The option to choose to use Google Colaboratory Notebooks or an Anaconda installation using Jupyter Notebooks.
* Additional datasets presented as case studies that focus on business applications added in addition to the existing case studies on other interesting topics.

One can find data science offered by departments such as computer science,
math or statistics, as well as business, 
so this edition strives to appeal
to the interests of students in each of these disciplines.
Of course, the applications of data science
are even broader and have broad application across the entire curriculum.
Our best hope is that the second edition of this text
can be used for courses in Data Science, Data Analytics, Business Analytics,
and possibly beyond!

We hope you like it and would love to hear from you!


Preface from the First Edition
------------------------------

by Brad Miller

It is said that the most important characteristic of a data scientist is curiosity.  Curiosity has certainly led me on a path of discovery throughout the world of data science and many fascinating data sets that I have encountered.  So, the premise of this book is to let the data sets lead you to learning.  The best and most interesting way to learn is to find some data and then begin to ask questions about it an analyze it, visualize it, and then write down new questions that have occurred to you as you have been doing your initial analysis.

This is how I organized the first two data science courses I ever taught, and surprisingly it worked.  In fact it worked so well that I would never want to teach it any other way.  Nevertheless it may not be clear from a high level look at the table of contents what this course covers and the learning goals it strives to achieve.  So let me lay it out for you in a different organization.


Learning Objectives
-------------------

* Articulate the data science processing pipeline
* Extract data using SQL
* Gather data from the Internet using web API's and screen scraping
* combine data from different sources
* Clean the data
* Handle missing data/finding outliers/fixing data
* Normalize and rescaling data
* Visualize the data
* Translate questions to analysis and analysis to interesting stories
* Analyze data

  * Single variable regression, logistic regression
  * Market basket analysis
  * Cohort analysis
  * Sentiment analysis, exposure to Bayes Theorem
  * Time series
  * Geographic analysis
  * Simulations, Monte Carlo

* Understand statistical significance and how to test for it using practical simulation techniques.


More Traditional Topic Outline
------------------------------

* Data Gathering

  - Using Web APIs
  - reading CSV files
  - Screen Scraping
  - Reading data from relational databases with SQL

* Data Munging

  - dealing with missing data
  - string processing
  - regular expressions
  - re-encoding data (one-hot)
  - re-scaling data

* Data Querying

  - filter
  - group by and aggregation
  - joining
  - sorting
  - reshaping
  - pivoting

* Analytical techniques

  - Linear Regression
  - Sentiment analysis
  - Market basket analysis
  - Cohort analysis
  - Time series

* Visualization

  - Understanding Distributions

    - Histogram
    - Box and whisker plot
    - Violin plot

  - Understanding relationships

    - scatter plot
    - bubble plot
    - heat map
    - Network diagrams
    - chord charts

  - Making Comparisons

    - bar chart / stacked bar chart
    - line chart
    - spider plot

  - Geographic analysis

    - Choropleth maps

Before you Clone this Repository install git-lfs
------------------------------------------------

There are a number of large data files in this book.  You need to enable git-lfs or when you clone you will just get stubs of the data files and things will break all over the place.

Before you build install the packages in requirements.txt
---------------------------------------------------------

This book also uses a number of additional packages that the regular runestone command does not include.  Please update your virtual environment.

Course Outline
--------------

[Week 1-2] --  Module 1
-----------------------

* Spreadsheets. Ex: Environmental studies, weather, happiness * data on countries
    - Descriptive statistics
	  - Charts: Scatter plots, box plots, line plots, histograms

* Using functions, including vlookup 
* Optimization using Solver

		

[Weeks 3-4] --  Module 2
------------------------

Review of Frequency Analysis for Textual Data. Data from United Nation dataset.

* Brainstorming/Generating questions: What were hot topics? What topics are common?
* Using Word Cloud & textatistic library in Python
* Using Web APIs 
* Join two datasets 

End-of-Module Exercise: Pick your favorite out-of-copyright data repository, and analyze character references.  Project Gutenberg.

* Module Intro (1 day) 
    - Loading files
    - This will be good review for python usage, e.g. reading files, working with dictionaries, etc.
    - Give an example of a question on something simple: what were important topics discussed in 1970? 
    - From this dataset, ask students what other questions would they want to explore, jot down on the board.  Add seeded questions to the board (from facilitator guide).
    - Segue into answering student-driven questions using Pandas; framing Pandas as a way to address pain felt earlier

* Pandas Intro
    - Prework: Watch Tutorials to get intro to Pandas:  https://www.youtube.com/watch?v=5JnMutdy6Fw 
    - Data Exploration Exercise #1 (Do this, what happened?, modify it, repeat):
    - Load data into data frame
    - Use filtering to see only the data from 1970)
    - see only data from 1970 from U.S.
    - Group By Year
    - Group By Country
    - Answer one of the questions you generated above, using some of the things you just learned/explored.

* Data Exploration #2: Quantify Text Data using 
    - Use wordcloud to create a visual, introduce that it’s minor data cleaning (removes ‘and’, ‘the’)
    - Use textatistic to assign a number to each row (add a column to your dataset)
    - Instructor-led debrief to review solution(s) and relay tips
    - Plot the complexity calculated

* Screen Scrape CIA data
    - CIA data is available online but not very convenient.  The CSV file we have is from 2006 so is quite outdated.  We would like to update this data.
    - Tutorial using requests python module
    - https://towardsdatascience.com/data-analytics-with-python-by-web-scraping-illustration-with-cia-world-factbook-abbdaa687a84

* Data Exploration #3: 
    - Add continent, region, GDP, life expectancy to our dataset
    - Create a simple visualization using newly added data (e.g. showing each country on the map with life expectancy)
    - Save the dataset by exporting to CSV so that you don't have to pull the data again

[Weeks 5-6] Module 3
--------------------

* Review of Frequency Analysis for Numeric Data. A numeric-based exercise from say DataUSA, pop culture (movie gross?)
	- Brainstorming/Generating questions: What were hot topics? What topics  are common?
	- Reading CSV/JSON
	- Handle missing data
	- Normalize the data
	- Correlation
	- Regression or classification
	- Exercise: TBD

[Week 7-8]  Midterm Project Weeks  
---------------------------------

Work in pairs, choose your dataset
In-class work on projects -- practice applying concepts from modules above

[Week 8-9]  Module 4
--------------------

Predictive -- simple recommender system. Ex: Insta-cart shopping basket recommendation; MovieLens data;  beer & diapers story; movies/music/books.
  - Correlation
  - Pull in Heat maps
  - SQL basics
  - Bias

[Week 10-11] Module 5  
---------------------

* Time Series/Historical Data Analysis.  Ex: Hamburger prices
    - Currency converting
    - Histograms
    - Sampling
    - Hypothesis testing

[Week 12, Holiday Break, TBD & movable] Fun Model + Choosing Visualizations
---------------------------------------------------------------------------

* Simulation -- Monte Hall -- 3 Doors, Prize
* Choosing between chart types for reports
* Dice or Roulette simulation
* Extra alternatives: Cohort Analysis

[Week 13-14]  Final Project & Presentation Week
-----------------------------------------------
Work in pairs, choose your dataset
Presentations (possibly a poster fair) & feedback