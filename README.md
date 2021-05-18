# Predicting temperature-dependent Vickers hardness

## Model overview
This model demonstrated an efficient and accurate machine-learning method to directly predict a material's experimentally measured temperature-dependent Vickers hardness.
![reg](/regressionplot-01.png)

## Table of Contents

- [Citations](#citations)
- [Prerequisites](#prerequisites)
- [Usage](#usage)
- [Authors](#authors)

## Citations

To cite temperature-dependent Vickers hardness predictions, please reference the following work:

Zhang. Z and Brgoch. J, Determining Temperature-Dependent Vickers Hardness with Machine Learning, in preparation.

##  Prerequisites

This package requires:

- [pymatgen](http://pymatgen.org)
- [XGBoost](https://xgboost.readthedocs.io/en/latest/#)
- [scikit-learn](http://scikit-learn.org/stable/)
- [pandas](https://pandas.pydata.org/pandas-docs/stable/index.html)
- [NumPy](https://docs.scipy.org/doc/numpy/index.html)
- [ASE](https://wiki.fysik.dtu.dk/ase/index.html)

## Usage

Note: The training dataset used in this work is provided in the form of pickle files, please see 'trainingset_x.p' and 'trainingset_y.p'.

To get the prediction for any crystal structure of interest, simply get the CIF file and direct the script model_soap.py to find the CIF file.

## Temperature and load dependence
This model is able to take two external factors into consideration: temperature (K) and applied load (N), making predictions of the same structure at different temperature/load.
