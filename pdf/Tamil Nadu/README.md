Media bullentins

## Query to get the updated details in WIkidata ##
SELECT ?item ?label ?publication_date ?number_of_pages ?full_work_available_at WHERE {
  ?item wdt:P31 wd:Q88163834.
  SERVICE wikibase:label {
    bd:serviceParam wikibase:language "en".
    ?item rdfs:label ?label.
  }
  ?item wdt:P921 wd:Q87821841.
  OPTIONAL { ?item wdt:P577 ?publication_date. }
  OPTIONAL { ?item wdt:P1104 ?number_of_pages. }
  OPTIONAL { ?item wdt:P953 ?full_work_available_at. }
}
ORDER BY DESC(?publication_date)
