# Multi-omics data integration

This repository contains materials for **Multi-omics data integration** hackathon for [#NGSprint2021](https://ngschool.eu/ngsprint).<br>
Follow recorded lectures on [Youtube](https://www.youtube.com/NGSchoolEU)

Michael Love Repo on Multiomics [Tools and packages](https://github.com/mikelove/awesome-multi-omics)<br>

## Literature to refer

1. [Evaluation and comparison of multi-omics data integration methods for cancer subtyping](https://journals.plos.org/ploscompbiol/article?id=10.1371/journal.pcbi.1009224)
2. [Comparison of Beta-value and M-value methods for quantifying methylation levels by microarray analysis](https://bmcbioinformatics.biomedcentral.com/articles/10.1186/1471-2105-11-587)


### Running the tutorial materials

To run the tutorial materials you will need:

1. The Jupyter notebook with the R language support:

  - Jupyter Notebook [(installation information)](https://jupyter.org/install)
  - R from CRAN-R [(download from here)](https://cloud.r-project.org)
  - IRKernel which enables the usage of R from the notebooks [(see tutorial here)](https://towardsdatascience.com/how-to-run-r-scripts-in-jupyter-15527148d2a)

2. R packages (see the instructions in the *set_up.R* file)

3. python3.6+ [(download from here)](https://www.python.org/downloads)

4. SUMO: the subtyping tool for multi-omic data [(installation information)](https://github.com/ratan-lab/sumo)

## Exploring the AML cancer data
1. Learn about the DNA methylation data from [TCGA](https://www.youtube.com/watch?v=Jg8MiFamLfg)
2. Log transformation of [RPKM values](https://www.biostars.org/p/344925/)
3. Convert .ipnyb file to .Rmd file using `rmarkdown:::convert_ipynb("1_Data_exploration.ipynb", output = xfun::with_ext("1_Data_exploration.ipynb", "Rmd"))`

The mRNA data contains rows (gene symbols and EntrezID) and column contain samples. The sample barcodes can be understood from [here](https://docs.gdc.cancer.gov/Encyclopedia/pages/TCGA_Barcode/)

![](https://docs.gdc.cancer.gov/Encyclopedia/pages/images/barcode.png)
### Resources & Aknowledgements

A significant portion of included materials was created based on very informative "Multi-omics Analysis" chapter by Jonathan Ronen from the "Computational Genomics with R" book available [here](https://compgenomr.github.io/book/multiomics.html) under the [Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License](https://creativecommons.org/licenses/by-nc-sa/4.0/).

The Acute Myleoid Leukemia (AML) is availble [here](http://acgt.cs.tau.ac.il/multi_omic_benchmark/download.html). The data was pre-processed and made available as a part of following paper: *Rappoport, N., & Shamir, R. (2018). Multi-omic and multi-view clustering algorithms: review and cancer benchmark. Nucleic Acids Research, 46(20), 10546–10562. https://doi.org/10.1093/nar/gky889*

SUMO package documentation detailing example usage is available [here](https://python-sumo.readthedocs.io/en/latest)
