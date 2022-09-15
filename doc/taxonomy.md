**node_id** (compulsory): Node identifier. This field should be programatically assigned, not edited.

**cell_type_name** (compulsory): "The primary name/symbol to be used for the cell type defined by this node."

**parent_node_id** (compulsory): ID of parent node. This field should be programatically assigned, not edited.

**synonyms** (optional): A list of alternative names for this cell type. Separate entries with a '|'.
Do not use terms here that are much narrower or broader than the cell type being described.

**synonym_provenance** (optional): Each entry in the synonyms field should have a corresponding entry here, 
either the DOI of a supporting publication or the editor's ORCID.  Multiple entries should be separated by a '|'.

**classification_ontology_id** (compulsory): The ID of a cell ontology term that classifies the cell type defined by this node. 

**classification_ontology_name** (compulsory): The name of the ontology term in the classification_ontology_id columns. 
