<img src="cimcb_logo.png" style="width: 160px; float: right;">

# README.md - `SI_Mendez_etal_2019`   

<br/>

<p align="justify">This repository contains the supplementary information for the journal article, "Expanding the Interpretation and Visualisation of Artificial Neural Networks in Metabolomics using the Structural Equivalence to Partial Least Squares Regression". There are two types of workflows included in this repository: standardised partial least squares (PLS) regression workflow, and a equivalent artificial neural network workflow. In addition to these workflows (and data), the outputs of the variable importance metrics are stored and evaluated for the comparable quantification between PLS (VIP and Coefficients) and ANN (Garson's Algorithm and Connection Weight Approach) using Spearman's Rank-Order Correlation in another notebook.</p>

<p align="justify">Two previously published metabolomics datasets are used as examples of the standardised PLS workflow and the proposed equivalent ANN workflow. The first, by <a href="https://www.nature.com/articles/bjc2015414">Chan et al. (2016)</a> is a urine NMR dataset comprised of 149 named metabolites, publicly available on Metabolomics Workbench (Study ID: <a href="http://dx.doi.org/DOI:10.21228/M8B10B">ST0001047</a>). Two classes were used: gastric cancer (n=43) vs. healthy controls (n=40). The second, by <a href="https://doi.org/10.1371/journal.pgen.1004801">Ganna et al. (2014)</a> and <a href="https://doi.org/10.1101/002782">Ganna et al. (2015)</a> is a plasma LC-MS with 189 named metabolites, publicly available on Metabolights (Study ID: <a href="https://www.ebi.ac.uk/metabolights/MTBLS90">MTBLS90</a>), and samples were split into two classes by sex: males (n=485) and females (n=483).</p>

<p align="justify">In this study, due to the structural equivalence with PLS, a shallow (2-layer) ANN is used. Provided the success of this approach to visualisation and interrogation, it may then be possible to adapt this further to deeper ANN architectures. This shallow (2-layer) ANN architecture has a hidden layer consisting of multiple neurons (n = 2 to 6) with a sigmoidal activation, and an output layer consisting of a single neuron with a sigmoidal activation function.</p>

<p align="justify">The standardised PLS workflow and the proposed equivalent ANN workflow include the following steps: hyperparameter optimisation, building and training the model, bootstrap resampling of the model, model evaluation, and model visualisation. All steps and accompanying visualisation methods are described in the workflows above the corresponding code cell. These workflows were implemented using the Python programming language, and are presented as Jupyter Notebooks. There are three ways to that these can be accessed: as a static html, in the cloud (using Binder), or on downloaded and run on a local machine.</p>

<br/>

### *To open notebooks as a static file:* 
-  [Method: PLS-DA; Dataset: ST001047](https://kevinmmendez.github.io/metabviz/static/PLSDA_ST001047.html)
-  [Method: ANN-SS; Dataset: ST001047](https://kevinmmendez.github.io/metabviz//static/ANNSigSig_ST001047.html)
-  [Method: PLS-DA; Dataset: MTBLS90](https://kevinmmendez.github.io/metabviz//static/PLSDA_MTBLS90.html)
-  [Method: ANN-SS; Dataset: MTBLS90](https://kevinmmendez.github.io/metabviz//static/ANNSigSig_MTBLS90.html)

<br/>

### *To launch the notebooks in the cloud (using Binder):* 
-  [Method: PLS-DA; Dataset: ST001047](https://mybinder.org/v2/gh/kevinmmendez/metabviz//master?filepath=notebook/static/PLSDA_ST001047.ipynb)
-  [Method: ANN-SS; Dataset: ST001047](https://mybinder.org/v2/gh/kevinmmendez/metabviz//master?filepath=notebook/static/ANNSigSig_ST001047.ipynb)
-  [Method: PLS-DA; Dataset: MTBLS90](https://mybinder.org/v2/gh/kevinmmendez/metabviz//master?filepath=notebook/static/PLSDA_MTBLS90.ipynb)
-  [Method: ANN-SS; Dataset: MTBLS90](https://mybinder.org/v2/gh/kevinmmendez/metabviz//master?filepath=notebook/static/ANNSigSig_MTBLS90.ipynb)

<br/>

### *To download and run notebooks on a local machine*

<i>Note: If you are using Windows, you need to install git using the following:<i/> [Git for Windows](https://gitforwindows.org/)

1. Open Terminal on Linux/MacOS or Command Prompt on Windows
2. Enter the following into the console (one line at a time)

```console
git clone https://github.com/kevinmmendez/MetabViz
cd MetabViz
conda env create -f environment.yml
conda activate MetabViz
jupyter notebook
```

<br/>
