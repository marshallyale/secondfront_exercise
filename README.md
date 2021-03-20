**SecondFront Data Exercise:**

To accomplish this exercise, I built a COVID-19 information sheet from 3 open source APIs to dig down into how COVID-19 affected different regions and subregions.

https://about-corona.net/documentation - Historical information per Country
https://covidtracking.com/data/api/version-2 - More information specific to the United States
https://fabian7593.github.io/CountryAPI - Information about different Countries including region.

To get the IP address of the neo4j instance in the docker container, run:
`sudo docker container inspect exercise_neo4j | grep IP`
This will have to be the IP used in Jupyter Notebook to connect to the neo4j database.
