# Data and code for "What are the Effects of Utah Income Tax Rate Cuts?"
This repository contains the data and code for the analyses in the *Research in Focus* article by [Richard W. Evans](https://sites.google.com/site/rickecon) (@rickecon) entitled "What are the Effects of Utah Income Tax Rate Cuts?".

## Files and directories in the repository
This repository contains the following items:
* [`UT_RateCut.ipynb` Jupyter notebook](UT_RateCut.ipynb). An executable notebook you can use to replicate all the analyses in the article and creation of output and figures. You can either clone or download this repository and run the `UT_RateCut.ipynb` notbook on your machine locally. Or you can [open it in Google Colab](https://colab.research.google.com/drive/1zDjvfUdIfxA8piAHBJwceslVoRzspKBO?usp=sharing) and run the notebook from your browser in which all the software and computation is hosted in the cloud. To run this notebook locally on your machine, do the following steps:
    * Fork and clone (or download) the https://github.com/TheCGO/UT-RateCut repository
    * In your computer's terminal, navigate to the directory of the `UT-RateCut` repository on your local machine.
    * Create the conda environment `ut-ratecut-dev` by typing the following command: `conda env create -f environment.yml`
    * Activate the `ut-ratecut-dev` conda environment by typing the following command: `conda activate ut-ratecut-dev`
    * Fork and clode (or download) the https://github.com/TheCGO/fiscalsim-us repository.
    * With the `ut-ratecut-dev` conda environment activated, navigate to the folder of the `fiscalsim-us` repository on your local machine.
    * With the `ut-ratecut-dev` conda environment activated, install the `fiscalsim-us` package into this conda environment by typing the following command:
        * For Mac OS: `pip install -e .'[dev]'`
        * For Windows: `pip install -e ."[dev]"`
        * For Linux: `pip install -e .`
    * This should allow your notebook to run while this conda environment is activated.
* [`/images/` directory](images/). This folder contains the `.html` files for teh dynamic visualizations in the paper and created in the notebook and the corresponding static `.png` image files.
* [`/data/` directory](data/). This directory contains the data used in the analyses in the article--PEW total balances and rainy day fund balances historical data for all 50 states.
    * [`/data/calculations.xlsx`](/data/calculations.xlsx).
    * [`/data/fig1_source.csv`](/data/fig1_source.csv). Source data for Figure 1 in the paper.
    * [`/data/fig2_source.csv`](/data/fig2_source.csv). Source data for Figure 2 in the paper.
    * [`/data/ReservesBalancesData.xlsx`](data/ReservesBalancesData.xlsx). PEW Charitable Trusts historical data on all 50 states total balances and rainy day fund balances from 2000 - 2022. "[Fiscal 50: State Trends and Analysis: Reserves and Balances](https://www.pewtrusts.org/en/research-and-analysis/data-visualizations/2014/fiscal-50#ind5)", updated December 16, 2022 (accessed Dec. 31, 2022). Data can be downloaded from the PEW site from this URL (https://www.pewtrusts.org/-/media/data-visualizations/interactives/2016/fiscal-50/docs/2013/ReservesBalancesData.xlsx?v=202210).
