# EDOME
Extended DOME (data, optimization, model, and evaluation)

EDOME computes metrics specified by Walsh et al. 2021 to predict the performance of regression models of biological systems. Our goal is to assess the Euclidean distance (L2 norm) of machine-learning models from an ideal model with the following coordinates: mean absolute error (MAE) = 0.0, coefficient of determination (R2) = 1.0, and Root-mean squared error (RMSE) = 0.0. We also have metrics combining the DOME strategy with the estimation of Spearman's (r) and Pearson's (r) correlations named EDOME (Extended DOME).  
The metrics EDOMEr2 and EDOMEr add r2 (squared Pearson correlation) and r (Spearman correlation) to the Euclidean distance equation (DOME), respectively. The last metric is EDOME. We take the following metrics: r2, r, RMSE, MAE, and R2. The goal is to evaluate the distance of a machine-learning model from an ideal model with the following coordinates: r2 = 1.0, r = 1.0, RMSE = 0.0, MAE = 0.0, and R2 = 1.0. 

Reference
Walsh I, Fishman D, Garcia-Gasulla D, Titma T, Pollastri G; ELIXIR Machine Learning Focus Group; Harrow J, Psomopoulos FE, Tosatto SCE. DOME: recommendations for supervised machine learning validation in biology. Nat Methods. 2021; 18(10): 1122-1127.   <a href="https://pubmed.ncbi.nlm.nih.gov/34316068/">PubMed</a>

<H2>Installing EDOME (Linux)</H2>

You should type all commands shown here in a Linux terminal. The easiest way to open a Linux terminal is to use the Ctrl+Alt+T key combination.

<B>Step 1.</B> Download Anaconda Installer for Linux or newer.

Go to the directory where you have the installer file and type the following commands:

<pre><I>    chmod u+x Anaconda3-2021.11-Linux-x86_64.sh
    ./Anaconda3-2021.11-Linux-x86_64.sh</I></pre>

Follow the instructions of the installer. You may use a newer installer, but be sure to have the right installer in the above command lines.

<B>Step 2.</B> To run EDOME properly, you need Scikit-Learn 1.4.0. To be sure you have version 1.4.0, open a terminal and type the following commands:

<pre><I>    python3 -m pip uninstall scikit-learn
    python3 -m pip install scikit-learn==1.4.0</I></pre>

<B>Step 3.</B> Download <a href = "https://github.com/azevedolab/EDOME/blob/main/edome.zip" title="SAnDReS 2.0.0">edome.zip</a>. Copy the EDOME zipped directory (edome.zip) to wherever you want it and unzip the zipped directory.

Type the following command:

<pre><I>    unzip edome.zip</I></pre>

We have a CSV file (bind_Ki_test_set.csv) and three input files (edome.in, edome_plot1.in, and edome_plot2.in) besides the Python scripts in the zipped folder. 

cd to edome directory then, type:

<pre><I>python3 edome.py edome.in</I></pre>

EDOME will generate the following plots (bind_Ki_test_set_log(RMSE)_log(MAE).png and bind_Ki_test_set_r2_rho.png) and a csv file (bind_Ki_test_set_stats.csv).

