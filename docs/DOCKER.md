Install ELK via DOCKER
===
(and what you should see) 
-- 

ES and Kibana:
--------------
The initial docker-compose.yml was created from this starter
https://www.elastic.co/guide/en/elastic-stack-get-started/current/get-started-docker.html

note: none of the security / TSL stuff was attempted, just the first ES/Kabana.  

- curl -X GET "localhost:9200/_cat/nodes?v&pretty"
- http://localhost:9200/
- http://localhost:5601/app/kibana_overview#/

Filebeat:
---------
- docker-compose config I'm using right now:
https://github.com/shazChaudhry/docker-elastic/blob/master/filebeat-docker-compose.yml
- How to Tune Elastic Beats Performance: A Practical Example with Batch Size, Worker Count, and More:
https://www.elastic.co/blog/how-to-tune-elastic-beats-performance-a-practical-example-with-batch-size-worker-count-and-more?blade=tw&hulk=social
- Misc: https://www.elastic.co/guide/en/beats/filebeat/7.10/running-on-docker.html