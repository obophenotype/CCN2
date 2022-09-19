## Glossary

Adapted from Glossary (Table 1) in  "Common cell type nomenclature for the mammalian brain." Miller et al., 2020 (doi:10.7554/eLife.59928)

* **Cell taxonomy**: A Set of quantitatively derived clusters of data about single cells, defined by a specific computational algorithm on a specific dataset(s). Taxonomies are given a unique label and can be annotated with metadata about the taxonomy, including details of the algorithms and relevant cell and cell set IDs.  A taxonomy may be flat, or hierarchical. Hierarchical taxonomies are typically single inheritance (each cluster has only one parent). *E.g.* Any clustering result in a cell type classification manuscript

* **Dendrogram**: A representation of a single inheritance hierarchical taxonomy as a tree in which the length of each branch is proportional to the dissimilarity between sibling clusters

* **Marker gene(s)**: A gene (gene set) which, when expressed in a cell, can be used to accurately assign that cell to a specific cell set.
*e.g.* GAD2; PVALB; CHODL

* **Taxonomy ID**: An identifier uniquely tagging a taxonomy of the format CCN[YYYYMMDD][#]. e.g. CCN201910120

* **Cell set**: Any tagged group of cells in a taxonomy. This includes groups of cells that define cell types, groups of cell types, and potentially other informative groupings (e.g., all cells from one donor, organ, cortical layer, or transgenic line).
Examples: A cell type; a group of cell types; all cells from layer two in MTG; all cells from donor X

* **Provisional cell type**: A cell type defined by a cell set.  Another way to put this is that a cell set provides the ground truth for defining a provisional cell type. Other cell types are determined to belong to this type or be related to it by some algorithm determining similarity (e.g. transcriptomic similarity).

* **leaf node (provisional) cell type**\*: A provisional cell type defined by a cell set that is a leaf node in a hierarchical clustering (e.g. L5 ET_1).

* **gross (provisional) cell type**\*: A provisional cell type defined by a cell set that is a leaf node in a hierarchical clustering (e.g. GABAergic neuron)

* **family (provisional) cell type**\*: A provisional cell type defined by a cell set that is an intermediate node in a hierarchical clustering.

* **reference taxonomy**: A taxonomy based on one or a combination of high-confidence datasets, to be used as a baseline of comparison for datasets collected from the same (or closely related) anatomical structure.

* **Cell set accession ID**: A unique ID for a cell set. This is derived from the Taxonomy_id by the appending a '_' followed by an integer. e.g. CS201910120_1

\* A note on the terms class, subclass, and type in CCN1: In CCN1 and least some of the literature using it, cell type is used to refer only to cell groupings defined by leaf node cell sets. Class is used to refer to cell groupings defined by very general cell sets in a hierarchical clustering.  SubClass (in some papers 'family') is used to refer to cell groupings defined by mid-level clusters - with position in the hierarchy chosen somewhat flexibly. The use of these terms is potentially confusing given the regular use of class and subclass in discussion of classification, we therefore prefer the terms leaf node, family, and gross cell type.
