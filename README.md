# covid-19-in-India
COVID-19 Media Bulletins from States of India.

Updating:

 Kerala (English & Malayalam)
 
 Tamil Nadu (English)
 
 Karnataka (English and Kannada)


This area is archieve of collections of Media bulletins form different states of India.

The media bulletins published by various state goverments are linked to Wikidata for references. The items that are created fore each state can be accessed by using sparql qery which is given in descriptions of each state.

#### For getting Media Bulletins of Kerala Government date wise (English and Malayalam)
##### Here is the query in SPARQL:
```SPARQL
SELECT ?item ?label ?publication_date ?full_work_available_at WHERE {
  ?item wdt:P31 wd:Q88163834.
  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
    ?item rdfs:label ?label.
  }
  ?item wdt:P921 wd:Q87429464.
  OPTIONAL { ?item wdt:P577 ?publication_date. }
  OPTIONAL { ?item wdt:P953 ?full_work_available_at. }
}
ORDER BY DESC (?publication_date)
```
#### For getting Media Bulletins of Tamil Nadu Government date wise (English)
##### Here is the query in SPARQL:
```SPARQL
SELECT ?item ?label ?publication_date ?full_work_available_at WHERE {
  ?item wdt:P31 wd:Q88163834.
  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
    ?item rdfs:label ?label.
  }
  ?item wdt:P921 wd:Q87821841.
  OPTIONAL { ?item wdt:P577 ?publication_date. }
  OPTIONAL { ?item wdt:P953 ?full_work_available_at. }
}
ORDER BY DESC (?publication_date)
```
#### For getting Media Bulletins of Karnataka Government date wise (English and Kannada)
##### Here is the query in SPARQL:
```SPARQL
SELECT ?item ?label ?publication_date ?full_work_available_at WHERE {
  ?item wdt:P31 wd:Q88163834.
  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
    ?item rdfs:label ?label.
  }
  ?item wdt:P921 wd:Q87763738.
  OPTIONAL { ?item wdt:P577 ?publication_date. }
  OPTIONAL { ?item wdt:P953 ?full_work_available_at. }
}
ORDER BY DESC (?publication_date)
```
#### For getting Media Bulletins of Delhi Government date wise (English)
##### Here is the query in SPARQL:
```SPARQL
SELECT ?item ?label ?publication_date ?full_work_available_at WHERE {
  ?item wdt:P31 wd:Q88163834.
  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
    ?item rdfs:label ?label.
  }
  ?item wdt:P921 wd:Q87821864.
  OPTIONAL { ?item wdt:P577 ?publication_date. }
  OPTIONAL { ?item wdt:P953 ?full_work_available_at. }
}
ORDER BY DESC (?publication_date)
```
