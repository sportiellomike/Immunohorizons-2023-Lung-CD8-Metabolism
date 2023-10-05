# Immunohorizons-2023-Lung-CD8-Metabolism
 Analysis and data for 2023 Immunohorizons publication

# Overview
**Authors**: _Mike Sportiello, Alexis Poindexter,  Emma C. Reilly, Adam Geber, Kris Lambert Emo, and David J. Topham_\
**Maintainer**: Please contact Mike Sportiello at Sportiellomike@gmail.com.

The code available here is to demonstrate reproducibility for all work in this manuscript. The metabolic modeling was created using the [COBRA Toolbox](https://opencobra.github.io/cobratoolbox/stable/) as well as other software including Matlab, Rstudio, Pycharm, and more. This code, to make it most reproducible, is set up with masterscripts--which call upon other scripts. In order for this work to be reproduced, it is essential that the scripts are run in the correct order, and files are located in the correct places. If you just want to use the constructed metabolic models, we have those saved and available so you don't have to rerun everything.

# Install
First, you must install the COBRA Toolbox, with directions on how to do so located [here](https://opencobra.github.io/cobratoolbox/stable/installation.html). I used COBRA Toolbox v 2.30.1 with gurobi solver v 9.1.1. Instructions on how to download and install gurobi solver are also located in the COBRA toolbox installation link, though usage of that specific solver is likely unncessary to perfectly reproduce these results.

# Rerunning our code
Run the code in the following order from the 'modellingcode' subfolder as your working directory:
* `masterscript-matlab.m`
	* make sure that you uncomment out the "writecbmodel" arguments in the code that take forever but are required if you want to remake them. Again, you can just go to the models folder and just download the models so you don't have to rerun the code. 
* `masterscript-python.py`
* To regenerate plots, run the R scripts in their folders listed below
	* `in vitro differentiation with metabolites`
	* `uptake experiments`
	* `transcriptomic analysis`

# Citation
If you use our code, we'd appreciate you citing us. The doi for citation can be found [here]().
