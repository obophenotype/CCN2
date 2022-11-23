# CCN2 - Developing a successor to the CCN taxonomy system

## CCN1

The Common Cell Type Nomenclature standard (Miller et al, 2020) is a standard for annotating, organising and linking cell type taxonomies built from clustering of single cell data based on some measure of similarity.  A taxonomy in this case may be a heirarchical or flat.  So far this has been applied to single cell transcriptomics, epigenomics, electophysiology data and morphlogy.  R dendrograms are the only supported heirarchical clustering input format.  These are single inheritance (each node/cluster has only one parent).  

The standard specifies a set of property key names applied to each cluster, including one for unique identifiers (applied according to a standard schema), one for a primary name for a (provisional) cell type defined by the cluster and others designed to be used for mapping between taxonomies based on the use of shared names (aliases).

A limited set of nomenclature recommendatations for cortical cell types was released with the initial schema.  

* Miller, J. A., Gouwens, N. W., Tasic, B., Collman, F., Van Velthoven, C. T. J., Bakken, T. E., Hawrylycz, M. J., Zeng, H., Lein, E. S., & Bernard, A. (2020). Common cell type nomenclature for the mammalian brain. ELife, 9, 1–23. https://doi.org/10.7554/eLife.59928

### Basic workflow 

(A much more detailed, practical workflow for CCN1 is described [here](http://htmlpreview.github.io/?https://github.com/AllenInstitute/nomenclature/blob/master/scripts/build_annotation_tables_SEAAD.nb.html).)

![image](https://user-images.githubusercontent.com/112839/203593004-2eb6d935-d092-4426-8a96-8a0acf970f00.png)


An R dendrogram object and taxonomy metadata are used as input to the [CCN R library](https://github.com/AllenInstitute/CCN/). The library annotates all clusters with an ID, following a standard schema and can also be used to populate the standard set of properties defined by the schema.  IDs are also written back to files assigning individual cells to clusters ().  This file may also contain further cell type annotations/names.

The results can be saved as a standard JSON representation of an R dendrogram, or as a CSV.  The CSV may be further modified with additional manual annotation and the addition of cross-cutting classification nodes (breaking single inheritance). 

R dendrograms are widely used for generating visualisations of taxonomies. The annotated versions resulting from the application of CCN are used for figure generation.


### Aims for CCN2: 
 - Split nomenclature recommendations from schema.
 - Support existing use cases and workflows - particularly figure generation
 - Improve robustness by using node and ontology ids in cross-referencing, rather than names/aliases.
 - Encourage the use of ontology terms where possible.
 - Support the inclusion of evidence and provenance
 - Allow for expressiveness, but keep compulsory fields to a minimum.
 
 
### Schema and Documentation:
A formal JSON schema can be found at [src/schema/schema.json](src/schema/schema.json).  However, we expect users to interact with this schema via flattened tables in an editor tool and available as reports.  Documentation, user guidance for those tables as well as examples can be found under [doc](doc).

Proposed CCN2 workflow

![image](https://user-images.githubusercontent.com/112839/203592749-40ac9def-8b7b-476c-90ad-a7ba05144908.png)



