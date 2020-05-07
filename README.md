# Interactive gene plots
Did you just run a clustering algorithm on some single-cell RNAseq or spatial transcriptomic data (e.g. Slide-seq)? Are you trying to interrogate the cluster assignments and interpret them in light of known marker genes? Try this interactive visualization code!

Remark: The interactive visualizations in this repo utilize [Altair](https://altair-viz.github.io/index.html) and [ipywidgets](https://ipywidgets.readthedocs.io/en/latest/index.html) and are broadly applicable to any high dimensional dataset where one wishes to examine cluster labels in a two dimensional representation and overlay the label information with the value of (informative) features.

**Coming soon!** Hippocampus example :)

## How do I run this?
There are two options:
* **Locally**

Note: This requires standard scientific Python 3 environment. A simple way of getting that is installing [Anaconda](https://www.anaconda.com/distribution/#download-section).

Run the following commands in your terminal:
```
git clone https://github.com/tudaga/interactive_gene_plots
cd interactive_gene_plots
jupyter notebook interactive_plots_scRNAseq_Slideseq.ipynb
```
* **Remotely** via Google Colab

Don't want to install anything, download the data or clone the repo? No problem! Click on <a href="https://colab.research.google.com/github/tudaga/interactive_gene_plots/blob/master/Interactive_plots_scRNAseq_Slideseq.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>.

## Intro 
The notebook [interactive_plots_scRNAseq_Slideseq.ipynb](https://github.com/tudaga/interactive_gene_plots/blob/master/Interactive_plots_scRNAseq_Slideseq.ipynb) goes over a Slide-seq cerebellum example. The content is:
1. Run a [standard scanpy clustering pipeline](https://scanpy-tutorials.readthedocs.io/en/latest/pbmc3k.html).
2. Explore the clustering outcome with standard non-interactive plots.
3. Explore it with interactive plots! :)

You can download more Slide-seq datasets [here](https://singlecell.broadinstitute.org/single_cell/study/SCP815/sensitive-spatial-genome-wide-expression-profiling-at-cellular-resolution#study-download).
