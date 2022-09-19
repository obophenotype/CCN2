## Taxonomy table

**cell_set_accession** (compulsory): Primary identifier of the cell set. This field should be programatically assigned, not edited.

**cell_type_name** (compulsory): The primary name/symbol to be used for the (provisional) cell type defined by this cell set.

**parent_cell_set_accession** (compulsory): The cell set accession of the parent cell set in the taxonomy. This field should be programatically assigned, not edited.

**synonyms** (optional): A list of alternative names for this cell type. Separate entries with a '|'. Do not use terms with a scope that is much narrower or broader than the cell type being described.

**synonym_provenance** (optional): Each entry in the synonyms field should have a corresponding entry here,  either the DOI of a supporting publication (in the form the form doi:10.1126/science.abj6641) or the editor's ORCID (in the form: ORCID:).  Multiple entries should be separated by a '|'.

**classification_ontology_id** (compulsory): The ID of a cell ontology term that classifies the cell type defined by this node.

**classification_ontology_name** (compulsory): The name of the ontology term in the classification_ontology_id columns.

# cross taxonomy mapping table

**cell_set_accession** (compulsory): Primary identifier of the cell set.

**cell_type_name** (compulsory): The primary name/symbol of the (provisional) cell type defined by this cell set.

**mapped_cell_set_accession** (compulsory): The accession (ID) of a cell set in a second taxonomy that this cell set maps to.

**mapped_cell_type_name** (compulsory): The name of the cell type corresponding to the mapped_cell_set_accession.

**evidence_comment** (compulsory): A free text description of the evidence supporting this mapping. If a similarity_score is include, please also include details of how this was calculated.

**similarity_score** (optional): A score recording the similarity between mapped nodes.

**provenance** (compulsory): ORCID of the person doing the mapping using the syntax ORCID:{orcid}.Optionally include supporting publication using DOIs of the form doi:{doi}

## location mapping table

**cell_set_accession** (compulsory): Primary identifier for cell set.

**cell_type_name** (compulsory): "The primary name/symbol to be used for the cell type defined by this cell set."

**ontology_term_id** (compulsory): The ID of an ontology term that refers to a brain region that this cell type is located in. Ideally this should be the ID of a term defined as a region in a standard atlas."

**ontology_term_name** (compulsory): Name of the term whose ID is recorded in the ontology_term_id field.

**evidence_comment** (optional): A comment describing the evidence for this location mapping

**supporting_data** (optional): A link to data supporting this location mapping.
