# COVID-19 Knowledge Graph

## kgCreation.ipynb 
  is the main notebook for merging CROssBAR and CoV-KGE. It also is the main notebook to create the URI's and nTriple RDF graph.

## mappingInChiKeys.ipynb
  is the main notebook to map all MeSH, ChEMBl, ChEBi and DrugBank compounds(drugs/chemicals) to InChi Keys. 
  
## bridgeDBmapping.rmd
  is the main markdown file to map uniprot identifiers to entrez identifiers. 
  
## covid_KGEs.ipynb
  contains the attempted to code to use DGL-KE to compute RotatE knowledge graph embeddings. Upon not being able to use it given a lack of personal understanding, I attempted to compute KGEs with the pipeline module from pykeen with little success. 
  
## covid_networkAnalysis.ipynb
  contains the work done to infer meaning from the knowledge graph. Some algorithms (closeness_centrality and jaccard) took extremely long to calculate and were performed in R. 
