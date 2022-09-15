# Documentation

## Editor table documentation
 
 Documentation here describes user-facing tables, intended to be edited with the help of tooling.
 These tables split the single-table representation of CCN1 into a small number of tables linked 
 by node ID as key. Tables are used here for ease of editing, visualisation and reporting. However, 
 the underlying sharable, master representation of the linked tables is JSON, defined in a JSON 
 schema on this repo under src/schema.
 
 In addition to documentation, we provide examples as TSVs.
 
 ## Table structure - commonalities
 
 All tables start with columns for node_id and node_name. The node_name is for reference only. 
 It should be automatically populated by editor tools.
 
 ### Editor tables
 
 [taxonomy](taxonomy.md): This is the core taxonomy table, recording name
 
 [cross_taxonomy_mapping](cross_taxonomy_mapping.md): This table records links between taxonomies, 
 e.g. a link between a taxonomy of human cell types and a taxonomy of marmoset cell types indicating
 potential homology between cell types based on transcriptomic similarity.
 
 [location_mapping](location_mapping.md): This table is used to record the locations in which 
 the cell type defined by the node is found, and the evidence for this.
 
 
 
 