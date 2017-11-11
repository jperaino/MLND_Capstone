# Machine Learning Engineer Nanodegree
## Capstone Proposal
Jim Peraino  
November 11th, 2017

## Proposal

### Domain Background

In the domains of architecture and urban planning, building typology is an often referenced idea when analyzing neighbordhoods, buildings, and public spaces. Historically, buildings have been classified in two primary ways: by form (or shape), and by use (what happens inside). In the early 19th century, the architect Jean-Nicolas-Louis Durand proposed the notion of architectural typology in his book Precis des Lecons d'Architecture (1). Since then, many efforts have been made to apply machine learning techniques to Urban Design and Architectural analysis, including with software such as GIS (2) and spatial recognition systems for identifying ideal sites for new development projects (3).

As an architect myself, I'm curious about ways that we can quantify qualitative information about buildings, and vice versa. There are relatively few datasets in the field of architecture, and establishing and automating methods for classifying buildings, in particular into qualitative categories, will be essential in this endeavor. Being able to classify a building as a certain typology enables many other kinds of analysis. This information can be used to assess the characteristics of a neighborhood, predict property values, identify areas for new development, or countless other tasks related to the built environment.

### Problem Statement

Databases of building typologies do not exist for most of the world. To exacerbate this problem, buildings often no longer limit themselves to the typical typologies (schools, homes, hospitals, churches, for instance), and instead, are often mixed-use. However, physical charactistics of buildings can be easily observed or deduced from satelite images (3). 

__The problem, then, is: How can we automate the process of classifying buildings into their respective typologies by analyzing this physical information?__

The problem is quantifiable and measurable because we can logically assess any individual building as to the makeup of its use. It is a problem that is replicable anywhere on earth that there are buildings, since google earth shows satelite images from which we can mine physical data.

### Datasets and Inputs

New York City's Department of City Planning puts out a dataset called The Primary Land Use Tax Lot Output (PLUTO),  which contain information about plots of lands, the characteristics of the buildings on that land, and various administrative districts. This dataset was obtained as a download from Kaggle (4). This dataset contains information for over 65,000 lots. 

While the dataset has roughly 80 variables for each lot, those of particular interest are:

__Physical Characteristics__
* Total Building Floor Area
* Lot Area 
* Number of Floors
* Lot Frontage
* Lot Depth
* Building Frontage
* Building Depth
* Floor Area Ration (FAR)

__Other Data__
* Commercial, Residential, Office, Retail, Factory, Storage, Garage, and Other Floor Area
* Building Class
* Zoning District

Since my goal is to use physical characteristics to classify buildings into typological groups, I will test different combinations of Physical Characteristics to see which best enable clustering of the data into building typologies. I will then compare the percentages of commercial/residential/office etc. floor areas in each cluster to better understand and evaluate the clusters.

### Solution Statement

Unsupervised learning can be used on this task. As was used in the Customer Segment project, this solution can follow the process of: Data Exploration, Data Preprocessing, Feature Transformation, Clustering, and drawing conlusions(5). For more detail, see the project design section. 

### Benchmark Model

Existing methods for classifying building typology us

In the case of this dataset, we 


### Evaluation Metrics

We would expect that the benchmark model 

### Project Design
_(approx. 1 page)_

TODO
-----------

References:

(1) https://books.google.com/books?hl=en&lr=&id=wilTAAAAcAAJ&oi=fnd&pg=PA1&dq=precis+durand&ots=hY1zElBwh2&sig=clePUvTcCCBGFLNlBVFp0j4XPJw#v=onepage&q=precis%20durand&f=false

(2) https://pdfs.semanticscholar.org/24c5/4f200302943cde042aee677956adc0b2498e.pdf

(3) http://certainmeasures.com/spatial_recognition.html

(4) https://www.kaggle.com/new-york-city/nyc-buildings

(5) Udacity MLND Customer Segment Project

