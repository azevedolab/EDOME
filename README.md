# EDOME
Extended DOME (data, optimization, model, and evaluation)

You find here the Jupyter Notebook for EDOME (edome_2d_plot.ipynb). This code reads an input file defining parameters to caculate Walsh (<a href="https://pubmed.ncbi.nlm.nih.gov/34316068/">Walsh et al., 2021</a>) metric. It evaluates the predictive performance of features and scoring functions against a defined target variable (e.g., pKi). The input file (edo.in) should be in the content directory during a Colab session. It is also necessary to upload a CSV file with columns for all features and a target variable. This code outputs a CSV file with the statistical analysis and a plot showing all features defines in the edo.in.

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

