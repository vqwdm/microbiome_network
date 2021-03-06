# microbiome_network
Automatic generation of colored networks, stacked bar plots, and zc-plots based on input parameters. 

I'd like to thank the Stack Overflow community for making this code possible, and I'd like to thank Josh Claypool (jtclaypool/microbiome) for constructing the core functions behind this code.

Josh wrote the functions behind network filtering and creation, cluster analysis of the networks, zc-plot, and stacked bar charts. My code is a wrapper of those functions, with some added plot-beautification modifications. Within-code comments attempt to explain the premise of each block of code. 

What this code does:

Tables of keystone taxa are generated according to math and parameters specified by Oleson et. al "The modularity of pollination networks" and resulting scatter plots
Raw network graph
Network graph colored by Phylum, nodes sized by degree, community clusters visualized as polygons around clusters.
Network graph colored by Family, nodes sized by degree, community clusters visualized as polygons around clusters.
Network graph colored by keystone taxa, nodes sized by degree, no community cluster visualization
Stacked bar charts of community cluster relative abundance per sample

Assumptions:

You like the autogenerated file names and figure title names I gave. I made these parameters objects within R, so you just need to change the objects to fit your desired name. 
The sample ID column in your metadata file is headered as "Label." It's easy to change that in my code
Your input file (named 'biom' in the code) is in the format that the sample data is in. I think this is the case. I dunno, I didn't generate the sequencing data nor did I analyze it.
You dont care about metadata. I didn't while I was writing this. So I cannot guarantee manipulating this code for analysis of other metadata will work out.

email me at cfmasarweh@ucdavis.edu for questions, concerns, frustrations, etc
