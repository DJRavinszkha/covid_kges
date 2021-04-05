# COVID-19 Knowledge Graph
Please rememeber to changet all the paths to your own. 
All of the files used can be downloaded at:
    https://zenodo.org/record/4662104#.YGp_ZRMzYc8

The TSV format of the KG (not the RDF graph) with scores can be downloaded at:
    https://zenodo.org/record/4662244#.YGsRDRMzYc8
    
  The scores for non-GNBR triples in CoV-KGE were assigned an arbitrary value of 0.2. 
  The mean of the scores for the GNBR triples in CoV-KGE was approximately 0.004.
  The scores for triples in CROssBAR were given an arbitrary value of 0.7. The reason for this is due to the fact that this KG was     constructed using actionable knowledge. 
  These scores can be used as weights in several calculations.

## kgCreation.ipynb 
  is the main notebook for merging CROssBAR and CoV-KGE. It also is the main notebook to create the URI's and nTriple RDF graph.

## mappingInChiKeys.ipynb
  is the main notebook to map all MeSH, ChEMBl, ChEBi and DrugBank compounds(drugs/chemicals) to InChi Keys. It does this by scraping (using beautifulSoup4, Selenium and fuzzywuzzy) the relevant database websites given the known information.
  E.g. MeSH ID ---> Name ---> CID ---> InChi Key
       ChEMBl OR ChEBi OR DrugBank ---> InChi Key
  
## bridgeDBmapping.rmd
  is the main markdown file to map uniprot identifiers to entrez identifiers. 
  
## covid_KGEs.ipynb
  contains the attempted to code to use DGL-KE to compute RotatE knowledge graph embeddings. Upon not being able to use it given a lack of personal understanding, I attempted to compute KGEs with the pipeline module from pykeen with little success. 
  
## covid_networkAnalysis.ipynb
  contains the work done to infer meaning from the knowledge graph. Some algorithms (closeness_centrality and jaccard) took extremely long to calculate and were performed in R. 
