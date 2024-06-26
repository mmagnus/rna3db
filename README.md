# RNA3DB

A dataset of non-redundant RNA structures from the PDB. RNA3DB contains:
- All RNA chains in the PDB, labelled with non-coding RNA families
- Non-redundant clustering of the above chains, suitable for training and benchmarking deep learning models

## Getting started
We provide periodically updated versions of RNA3DB in [JSON](https://en.wikipedia.org/wiki/JSON) format, along with several intermediate steps used to generate the files.

Additionally, as part of RNA3DB, we release the results of [Infernal](http://eddylab.org/infernal/) homology search on all RNA chains found in the PDB. For a short demonstration on how RNA3DB can be used to parse these files, see [tabular_demo](notebooks/tabular_demo.ipynb).

For more general help getting started, see RNA3DB's [Wiki](https://github.com/marcellszi/rna3db/wiki).

## Download
The latest version of RNA3DB can be found under [releases](https://github.com/marcellszi/rna3db/releases/latest/).

We provide the following files: 
- `rna3db-cmscans.tar.gz` [[Download](https://github.com/marcellszi/rna3db/releases/latest/download/rna3db-cmscans.tar.gz)]
    - Results of two-step Infernal homology seach on all RNA chains in the PDB
- `rna3db-jsons.tar.gz` [[Download](https://github.com/marcellszi/rna3db/releases/latest/download/rna3db-jsons.tar.gz)]
    - All [JSON](https://en.wikipedia.org/wiki/JSON) files generated by RNA3DB
- `rna3db-mmcifs.tar.gz` [~~Download~~] (**COMING SOON**)
    - Hierarchical folders of the training/testing sets containing single-chain [PDBx/mmCIF](https://en.wikipedia.org/wiki/Macromolecular_Crystallographic_Information_File) files 
    - Most convenient for getting started with training and testing using RNA3DB

## Generating the dataset from scratch
If you wish to build your own dataset from scratch, please follow see [Building RNA3DB from scratch](https://github.com/marcellszi/rna3db/wiki/Building-RNA3BB-from-scratch).
