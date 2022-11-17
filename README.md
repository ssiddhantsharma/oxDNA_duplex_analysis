# oxDNA_duplex_analysis
Take a look at the following papers for an idea of what kinds of things can be done with oxDNA: 

1. [Original oxDNA paper](https://aip.scitation.org/doi/10.1063/1.3552946)
2. [oxDNA analysis tools](https://academic.oup.com/nar/article/48/12/e72/5843822)
3. [Hairpins](https://academic.oup.com/nar/article/43/13/6181/2414254)
4. [A review of feature extraction from molecular simulations](https://pubs.acs.org/doi/10.1021/acs.chemrev.0c01195)

Clone oxDNA from the Github, follow the instructions in the installation section of the documentation (with Python bindings enabled and CUDA enabled if you have a GPU). I would suggest trying the [OXPY_Jupyter example](https://github.com/lorenzo-rovigatti/oxDNA/blob/master/examples/OXPY_Jupyter/literate_sim.ipynb)

# Description of files here for OxDNA Analysis tool(OAT):

1. Run [duplexfinder](https://lorenzo-rovigatti.github.io/oxDNA/oat/cli.html#duplex-finder) from the OAT command line. 
2. It uses a trajectory file called: CO1_v11_traj.dat and an input file for input simulation conditions called input_run.
3. The .top file gives the topology of the structure and how many nucleotide it has in. 

The output from duplex_finder is *newduplex.tsv* which we use for analysis. 
