# agriculture
Supplementary Material of Bargués-Ribera &amp; Gokhale, agriculture project


This folder contains the following Jupyter notebooks:

(1) EcoEvo_agriculture_1SEQ.ipynb

(2) EcoEvo_agriculture_MULTISEQ.ipynb

(3) EcoEvo_agriculture_10bestseq.ipynb

Notebook (1) contains the code for running the model for 1 rotation sequence. 
The sequence needs to be specified at the section "Sequence population", in the variable 'seq', as a combination of 'h1', 'h2' and 'h1_r'.
In the predefined scenario infection starts at time 0. The scenario can be changed by modifying 'pathogen true' (1 for T, 0 for F) and 'infection time' (any discrete time number in the range of the length of the sequence).
Plots for soil quality/cash yield and eco-evolutionary dynamics will be displayed for the defined sequence.

Notebook (2) contains the code for running the model for multiple rotation sequences of a certain length L. 
All possible combinations of length L (to be specified) will be created in the section "Sequence population".
In the predefined scenario infection starts at time 0. The scenario can be changed by modifying 'pathogen true' (1 for T, 0 for F) and 'infection time' (any discrete time number in the range of the length of the sequence).
The program will generate .csv outputs for each sequence, containing the sequence pattern in binaries for each crop type, the delta values, the soil quality and cash yield time series, and the fitness value.

Notebook (3) imports the output files of Notebook (2) and gives the best 10 rotation sequences for the variable of choice: yield, soil quality or virulence. 

With these files, one can replicate the results shown in the paper. If interested in the generation of any plot not explicitely included, contact bargues[at]evolbio.mpg.de. 
