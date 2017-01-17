# Customer Segmentation (Unsupervised Machine Learning)

Many companies today collect vast amounts of data on customers and clientele, and have a strong desire to understand the meaningful relationships hidden in their customer base. Being equipped with this information can assist a company engineer future products and services that best satisfy the demands or needs of their customers.

In this project, unsupervised machine learning is implemented to product spending data collected for customers of a wholesale distributor in Lisbon, Portugal, to identify customer segments hidden in the data.

## Getting started

### Install

Viewing this project requires **Python 2.7** and the following Python libraries installed:

- [NumPy](http://www.numpy.org/)
- [Pandas](http://pandas.pydata.org)
- [matplotlib](http://matplotlib.org/)
- [scikit-learn](http://scikit-learn.org/stable/)

You will also need to have software installed to run and execute a [Jupyter Notebook](http://ipython.org/notebook.html)

If you do not have Python installed yet, it is highly recommended that you install the [Anaconda](http://continuum.io/downloads) distribution of Python, which already has the above packages and more included. Make sure that you select the Python 2.7 installer and not the Python 3.x installer.

### Run

Download or Clone the `MLND-CustomerSegments` projects on to your computer. In a terminal or command window, navigate to the top-level project directory `customer_segments/` (that contains this README) and run one of the following commands:

```bash
ipython notebook customer_segments.ipynb
```  
or
```bash
jupyter notebook customer_segments.ipynb
```

This will open the Jupyter Notebook software and project file in your browser.

## Data

The customer segments data is included as a selection of 440 data points collected on data found from clients of a wholesale distributor in Lisbon, Portugal. More information can be found on the [UCI Machine Learning Repository](https://archive.ics.uci.edu/ml/datasets/Wholesale+customers).

Note (m.u.) is shorthand for *monetary units*.

**Features**
1) `Fresh`: annual spending (m.u.) on fresh products (Continuous);  
2) `Milk`: annual spending (m.u.) on milk products (Continuous);  
3) `Grocery`: annual spending (m.u.) on grocery products (Continuous);  
4) `Frozen`: annual spending (m.u.) on frozen products (Continuous);  
5) `Detergents_Paper`: annual spending (m.u.) on detergents and paper products (Continuous);  
6) `Delicatessen`: annual spending (m.u.) on and delicatessen products (Continuous);  
7) `Channel`: {Hotel/Restaurant/Cafe - 1, Retail - 2} (Nominal)  
8) `Region`: {Lisnon - 1, Oporto - 2, or Other - 3} (Nominal)

## Data Analysis Procedures

In this unsupervised machine learning project, data analysis was conducted in the following steps.  
First, a small subset of data was explored to determine if any product categories are highly correlate with one another.  
Second, the data was preprocessed by scaling each product category and then identifying (and removing) unwanted outliers.  
Third, PCA transformation was applied to the good, clean customer spending data, you will apply PCA transformations to the data and implement clustering algorithms to segment the transformed customer data.  
Finally, segmentation found with an additional labeling were compared and ways this information could assist the wholesale distributor with future service changes were reported.
