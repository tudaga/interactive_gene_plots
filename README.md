# interactive_geneexpression_plots
Interactive visualization of marker genes and clustering in Slide-seq and single cell RNAseq data.

**Coming soon!** Examples of other applications :)

Do you have an application where NMFreg might help deconvolve your composite measurements aided by a labeled reference? Send me an email!

## How do I run this?
There are two options:
* **Locally**

Note: This requires standard scientific Python 3 environment. A simple way of getting that is installing [Anaconda](https://www.anaconda.com/distribution/#download-section).

Run the following commands in your terminal:
```
git clone https://github.com/tudaga/NMFreg_tutorial
cd NMFreg_tutorial
jupyter notebook NMFreg_Tutorial_cerebellum_puck180430_6.ipynb
```
* **Remotely** via Google Colab

Don't want to download the data and clone the repo? No problem! Click on <a href="https://colab.research.google.com/github.com/tudaga/interactive_gene_plots/blob/master/Interactive_plots_scRNAseq_Slideseq.ipynb" target="_parent"><img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/></a>.

## Intro 
The notebook [NMFreg_Tutorial_cerebellum_puck180430_6.ipynb](https://github.com/tudaga/NMFreg_tutorial/blob/master/NMFreg_Tutorial_cerebellum_puck180430_6.ipynb) goes over a cerebellum example. The basic steps are:
1. Run [NMF](https://en.wikipedia.org/wiki/Non-negative_matrix_factorization) on a labeled single-cell RNA-seq cerebellum dataset to derive an interpretable basis.
2. Regress the Slide-seq beads onto the basis via [NNLS](https://en.wikipedia.org/wiki/Non-negative_least_squares) to deconvolve each bead into proportional contributins from each cell type.
3. *Bonus* Get a heuristic measure on the certainty that a bead contains mRNA from a single celltype.

If you want to learn more about NMF, watch my lecture on it [here](https://www.youtube.com/watch?v=9f4Rwt0yqr4).

## Reference
This work is featured in the flagship paper for [Slide-seq: A scalable technology for measuring genome-wide expression at high spatial resolution](https://science.sciencemag.org/content/363/6434/1463).


