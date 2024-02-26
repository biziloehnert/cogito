# Cognitive Task Ontology connecting CogAt with HED 

The aim of this project is an ontology that connects Tasks from [Cognitive Atlas](https://cognitiveatlas.org/) with [HED Tags](https://www.hedtags.org/display_hed.html). In other words, we define the terms for cognitive tasks by their relation to HED tags, e.g. Reading (covert) is equivalent to `(has some Quiet) AND (has some Read) AND (has some (Character or Nonword or Word or Sentence or Phrase))`, where `Reading (covert)` is a Task from Cognitive Atlas and `{Read, Quiet, Word, Character, Nonword, Word, Sentence, Phrase}` are HED Tags. 
The purpose of this ontology is to query partially annotated datasets by either a cognitive task or HED Tags. 

## Dependencies
We reuse existing OWL files of [Cognitive Atlas](https://data.bioontology.org/ontologies/COGAT/submissions/7/download?apikey=8b5b7825-538d-40e0-9e9e-5ab9274a9aeb) and [HED](https://gitlab.com/api/v4/projects/45068833/jobs/artifacts/main/raw/HED8.2.0.owl?job=generate-owl) by importing them to our connector ontology. The import might fail when opening it with the [Protege Editor](https://protege.stanford.edu/), then it is necessary to import it again. 

## Usage
To use this ontology just open the [owl file](connector-ontology-for-cogat-and-hed/connector_cogAt_HED.owl). 