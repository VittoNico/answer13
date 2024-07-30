## answer13
```sparql
PREFIX aop: <http://www.aopwiki.org/ontology/>
PREFIX skos: <http://www.w3.org/2004/02/skos/core#>
PREFIX rdf: <http://www.w3.org/1999/02/22-rdf-syntax-ns#>

SELECT ?chemicalEntity ?preferredName ?casID
WHERE {
  ?chemicalEntity rdf:type aop:ChemicalEntity .
  ?chemicalEntity skos:prefLabel ?preferredName .
  ?chemicalEntity aop:hasCASID ?casID .
}
```
