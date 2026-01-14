# EDOME (Extended DOME (data, optimization, model, and evaluation)
You find here the Jupyter Notebook for EDOME (edome_2d_plot.ipynb). This code reads an input file defining parameters to caculate Walsh (<a href="https://pubmed.ncbi.nlm.nih.gov/34316068/">Walsh et al., 2021</a>) metric. It evaluates the predictive performance of features and scoring functions against a defined target variable (e.g., pKi). The input file (edo.in) should be in the content directory during a Colab session. It is also necessary to upload a CSV file with columns for all features and a target variable. This code outputs a CSV file with the statistical analysis and a plot showing all features defines in the edo.in.
<br> </br>
<b>Reference</b>
<br> </br>
Walsh I, Fishman D, Garcia-Gasulla D, Titma T, Pollastri G; ELIXIR Machine Learning Focus Group; Harrow J, Psomopoulos FE, Tosatto SCE. DOME: recommendations for supervised machine learning validation in biology. Nat Methods. 2021; 18(10): 1122-1127.   <a href="https://pubmed.ncbi.nlm.nih.gov/34316068/">PubMed</a>

