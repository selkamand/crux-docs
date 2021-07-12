##############################
Using CRUX
##############################

This section is under construction

====================================================
Choosing your dataset
====================================================

At the top of all analysis modules is a drop down menu that can be used to select a dataset of interest.
By default, datasets available are from **TCGA**, **PCAWG**, or **ZERO** initiatives.

Custom datasets become available immediately after being imported using the **import data** module.

====================================================
Single Cohort Mode
====================================================
All analyses/visualisations described below characterise a single cancer cohort.

----------------------------------------------------
Cohort-level mutational summaries
----------------------------------------------------
The first step in examining a dataset is often to visualise key metrics that summarise the cohorts mutational profile.


If you want to learn about:
- The distribution of variant classifications (Missense | Nonsense | Frameshift | etc)
- The distribution of variant types (SNP | Ins | Del)
- The frequencies of each base change (e.g. A>T | A>C | A>G | T>A | etc)
- How many mutations are present in each sample (e.g. to identify whether hyper-mutators are present)
- The top N mutated genes

Simply scroll down to the <panelname> and select the <tabname>.


----------------------------------------------------
Creating Oncoplots
----------------------------------------------------
An oncoplot is one of the most useful tools available for summarising the mutational profile of a cancer cohort.


If you want to learn about:
- What genes are mutated in the greatest number of samples
- What types of mutations are present in these recurrently mutated genes
- What genes may be driving disease in each sample
- How sample-level metadata varies with mutational status of commonly mutated genes
- How mutations found in particular samples of interest differ from others

Simply scroll down to <panelname> and select the <tabname> tab.

I would strongly recommend taking the time to learn how to read this plot.
It is a simple yet reasonably effective method of interesting genes and samples.


**Interpretation**

Each column is represents a sample. Each row a gene. The color of each square indicates whether if a gene is mutated in a particular sample, and if so, what type of mutation was observed.

In the example below, we see that <genename> is mutated in samples <sample1,sample2 & sample3>, while the other samples do not have a mutant <genename>.
Further, <sample1> has a missense mutation in <genename>, while <sample2> has a frameshift mutation.


**What genes are shown**

Oncoplots show only the genes mutated in the greatest number of samples.
The number of genes shown can be adjusted using the <optionname>


**What can we learn from Oncoplots?**

The idea is that the genes most frequently mutated in a cohort have increased likelihood of being important to the disease state studied.
If you're looking at a somatic cancer dataset (like any of those available in CRUX), this idea certainly holds weight.

For example, lets examine the Glioblastoma multiforme dataset from TCGA.
If we look at the oncoplot, we see known drivers of GBM disease appear near the top, including

- PTEN
- TP53
- EGFR
- PIK3CA
- IDH1

We also see a lot of genes that are more likely to be artefacts than true disease drivers.
For example, since we sort variants by recurrence in our cohort, very long genes, such as **TTN** can wind up sneaking their way into the oncoplot without having been specifically selected for in the tumor sample.
Additionally, some genes tend to have high rates of somatic mutation completely independent of whether their in a tumor or healthy cells.
These 'Dubious' hits can be filtered out using the option shown below. More info about what constitutes a 'Dubious hit' is described in the `FAQ / What are 'dubious genes'?` section

To further distinguish frequently mutated non-driver genes from genes driving disease, see `Using External Analysis Platforms`

**Adding sample-level metadata annotations**

In the **options** panel below the oncoplot, there is a <optionname> drop-down which can be used to select sample-level metadata you want to annotate samples with.
The results are shown below.

The order of samples in the oncoplot can be sorted by the sample metadata.
This may help you identify patterns in how sample-level metadata associates with the mutational status of commonly mutated genes


**Using custom genesets**

Depending on the goals of your research, you may not be exclusively interested in genes with highly recurrent mutations.
For example, perhaps you want to screen a cohort for samples that have mutations in a set of genes associated with drug resistance.
We can select a custom list of genes to visualise using the <optionname> drop-down menu.


----------------------------------------------------
Somatic Coocurrence Matrix
----------------------------------------------------

If you want to learn about:

- What pairs of genes are **frequently** mutated in the same samples (co-occurance)
- What pairs of genes are **rarely** mutated in the same samples (mutual exclusivity)

Simply scroll down to <panelname> and select the <tabname> tab.

**Why might genes show co-occurance or mutual exclusivity**

Mutual exclusivity

1. Belong to distinct subtypes which have taken entirely different paths to developing a cancerous genome
2. Genes both belong a pathway that must be dysregulated, but mutation of one is enough to cause this dysregulation (no selective advantage for mutating multiple members of the same pathway)


Co-occurance

1. <todo>


----------------------------------------------------
Copy-Number Analysis
----------------------------------------------------

----------------------------------------------------
Using External Analysis Platforms
----------------------------------------------------




====================================================
Two-Cohort Mode
====================================================
----------------------------------------------------
Two-Cohort comparison
----------------------------------------------------
----------------------------------------------------
Two-Cohort module
----------------------------------------------------




====================================================
Creating Custom Cohorts
====================================================
----------------------------------------------------
Subsetting
----------------------------------------------------
----------------------------------------------------
Merging
----------------------------------------------------
