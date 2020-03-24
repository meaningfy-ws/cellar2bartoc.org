# Production of import package to deploy EU vocabularies assets on Bartoc.org

The process was imagined as a future component of a larger process.
The current implementation of the pipelines uses Linked Pipes ETL (https://etl.linkedpipes.com/).

#### **Folders:** 
* pipeline: Contains the JSONLD source of the pipeline
* output: Contains sample of resulted ADMS files in RDF and TTL formats


#### **Input:** 
* CELLAR SPARQL endpoint
  
#### **Output goals:**
* To generate CSV file in acordance with BARTOC.org template import format

### ETL pipelines description
* Phase-0 : Extract asset metadata from CELLAR, limmiting selection to specific asset types (THESAURUS and NAL) and formats (SKOS_CORE)
* Phase-1 : Generat CSV structure in acordance with BARTOC import template
* Phase-2 : Save file on local FTP


###Technical notes for the current implementation
input data: accesible thru CELLAR SPARQL endpoint
output data: ftp://localhost:22/data/out/
 
