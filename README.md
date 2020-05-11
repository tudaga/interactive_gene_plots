# Interactive gene plots
Did you just run a clustering algorithm on some single-cell RNAseq or spatial transcriptomic data (e.g. Slide-seq)? Are you trying to interrogate the cluster assignments and interpret them in light of known marker genes? Try the interactive visualization code in this repo!

# Demos
* **Highlight each cluster across different 2D representations of the data:**
![](interactive_legend.gif)

* **Annotate clusters by intersecting the expression of a gene with the cluster labels:**
  - Select a gene of interest (either select from a dropdown menu or type in a gene name);
  - Pay special attention to the bar plot on the very right -- it shows the enrichment of the cluster labels in the beads expressing the gene of interest making it easy to find the biological identity of a cluster;
  - Toggle between binary expression and color proportional to gene counts (gene count per bead info available by hovering the mouse tooltip);
  - Customizable lower bound on expression via a slider.
![](annotate_clusters.gif)

* **Select an area on one plot and watch it condition the rest of the plots on the selection:**
![](select_rectangle.gif)

* **Select points on one plot and see where they fall on the other plot:**
![](link_selection.gif)

**Remark:** The interactive visualizations in this repo utilize [Altair](https://altair-viz.github.io/index.html) and [ipywidgets](https://ipywidgets.readthedocs.io/en/latest/index.html) and are broadly applicable to any high dimensional dataset where one wishes to examine cluster labels in a two dimensional representation and overlay the label information with the value of (informative) features.

**Coming soon!** Turn the notebook into an interactive dashboard with [Voilà](https://voila.readthedocs.io/en/stable/index.html).

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
