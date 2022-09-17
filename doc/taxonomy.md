**cell_set_accession** (compulsory): Primary identifier for cell set.

**cell_type_name** (compulsory): "The primary name/symbol to be used for the cell type defined by this cell set."

**parent_cell_set_accession** (compulsory): Indentifier of a parent cell set.

**synonyms** (optional): A list of alternative names for this cell type. Separate entries with a '|'.
Do not use terms whose scope is much narrower or broader than the cell type being described.

**synonym_provenance** (optional): Each entry in the synonyms field should have a corresponding entry here, 
either the DOI of a supporting publication or the editor's ORCID.  Multiple entries should be separated by a '|'.

**classification_ontology_id** (compulsory): The ID of a cell ontology term that classifies the cell type defined by this node. 

**classification_ontology_name** (compulsory): The name of the ontology term in the classification_ontology_id columns. 
