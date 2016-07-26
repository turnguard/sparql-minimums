# sparql-minimums

run the following sparql query at this endpoint: http://sparql.turnguard.com/sparql
```
SELECT ?obs ?componentProperty ?obsValue FROM <http://labs.turnguard.com/scuba> WHERE {
                    ?obs a qb:Observation;
                         qb:dataSet/qb:structure/qb:component/qb:componentProperty ?componentProperty .
                    ?obs ?componentProperty ?obsValue
            }  ORDER BY ?obs ?componentProperty
```

open developer console (e.g. f12) and reload the page, output is written to the console.
