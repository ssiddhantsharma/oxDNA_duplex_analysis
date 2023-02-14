# oxDNA_duplex_analysis
Take a look at the following papers for an idea of what kinds of things can be done with oxDNA: 

1. [Original oxDNA paper](https://aip.scitation.org/doi/10.1063/1.3552946)
2. [oxDNA analysis tools](https://academic.oup.com/nar/article/48/12/e72/5843822)
3. [Hairpins](https://academic.oup.com/nar/article/43/13/6181/2414254)
4. [A review of feature extraction from molecular simulations](https://pubs.acs.org/doi/10.1021/acs.chemrev.0c01195)

Clone oxDNA from the Github, follow the instructions in the installation section of the documentation (with Python bindings enabled and CUDA enabled if you have a GPU). I would suggest trying the [OXPY_Jupyter example](https://github.com/lorenzo-rovigatti/oxDNA/blob/master/examples/OXPY_Jupyter/literate_sim.ipynb)

# Feature_Analysis
Notebook for feature analysis of oxDNA simulation results. 
1. The Google Colaboratory first installs oxDNA & oxDNA Analysis tools, then loads up trajectory, topology, and input file of the sequence in the mounted google drive directory, and generates nucleotide pairs through a modification of [duplex_finder.py](https://github.com/lorenzo-rovigatti/oxDNA/blob/master/analysis/src/oxDNA_analysis_tools/duplex_finder.py)
2. The features obtained from the simulation results are: **Sequence Length**, **Average of % dsDNA**, **Average of % ssDNA**, **Standard Deviation % dsDNA**, **Standard Deviation % ssDNA**, 	**# of dsDNA fragments**, **Standard Deviation of # dsDNA fragments**, **Relative Percentage Abundance of dsDNA/Sequence Length**.

3. The nucleotide pairs are transformed into a dataframe, and features are calculated for the given sequence simulation, alongwith recording the time for generating the pairs, and for pair analysis. 
