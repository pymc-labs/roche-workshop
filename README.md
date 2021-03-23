# Bayesian Data Analysis Course

## Abstract

The goal of the Bayesian Data Analysis course is to provide Roche staff the necessary knowledge and tooling to be able to utilize Bayesian methods effectively. 
The course will consist of eight 2-hour sessions spreadout across 4 days. The morning sessions will be held between 10:00 and 12:00 CET, and the afternoon sessions will be held between 13:00 and 15:00 CET. The course will be given on the following dates: March 24, 26, 29, and 31.

## Pre-training recommended learning material:

- [PyMC examples](https://docs.pymc.io/nb_examples/index.html)
- [Bayesian Analysis with Python](https://www.amazon.com/Bayesian-Analysis-Python-Introduction-probabilistic-ebook/dp/B07HHBCR9G)
- [PyMC3 port of Statistical Rethinking](https://github.com/pymc-devs/resources/tree/master/Rethinking_2)
- [Thomas Wiecki’s blog](https://twiecki.io/)
- [Learning Bayesian Statistics podcast](https://www.learnbayesstats.com/)
 
## Course outline:

1. Get-to-know session
  1. What is your motivation to attend this course?
  2. What type of problems would you like to solve?
2. Introduction to Bayesian modeling and PyMC3
  1. What is a Bayesian statistical model?
  2. Learning from data by updating beliefs (Prior & Posterior)
  3. A high-level introduction to the PyMC3 API
  4. Motivating examples
3. Regressions and Hierarchical Models 
  1. Bayesian GLMs in PyMC3
  2. Motivation and case studies
  3. Partial pooling and benefits
  4. Building hierarchical models
  5. Parameterizations and how it helps
4. MCMC for Practitioners
  1. How to get posteriors computationally
  2. The idea behind MCMC
  3. MCMC gotchas and diagnostics
5. Project 1
  1. Model a small dataset with a hierarchical model
  2. Assess model convergence
  3. Analyze learnt parameters
  4. Study predictive capacity
6. The Bayesian Workflow
  1. Prior choice and predictive checks
  2. Iterating models
  3. Scaling your data
  4. Posterior predictive checks
  5. Using the model
  6. Missing data imputation
  7. Model checking and comparison
7. Bayesian Mixture Models 
  1. What they are & when they are useful
  2. Mixture models in PyMC3
  3. Limits of mixture models
8. Project 2
  1. Work with a dataset provided by the Roche digital biomarkers team

## Setup

The main working environment for the course will be Roche's HPC cluster. However, you will also be able to setup a local environment where you will be able to run the course's material. To do this, you will need to first install [Anaconda](https://www.anaconda.com/products/individual#download-section) (Python 3.8) on your system.

The next step is to clone or download the tutorial materials in this repository. If you are familiar with Git, run the clone command:

```
git clone https://github.com/pymc-labs/roche-workshop.git
```

otherwise you can [download a zip file](https://github.com/pymc-labs/roche-workshop/archive/refs/heads/main.zip) of its contents, and unzip it on your computer.

The repository for this tutorial contains a file called `environment.yml` that includes a list of all the packages used for the tutorial. If you run:

```
conda env create -f environment.yml
```

from the main tutorial directory, it will create the environment for you and install all of the packages listed. This environment can be enabled using:

```
conda activate bayes_workshop
```

Then, you can start **JupyterLab** or **Jupyter notebook** to access the materials:

```
jupyter lab
```

