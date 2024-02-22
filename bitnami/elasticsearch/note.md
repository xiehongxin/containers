```shell

$ mkdir elasticsearch
$ cd elasticsearch
$ echo "http.host: 0.0.0.0" >> config/elasticsearch.yml

sudo docker run --name elasticsearch -p 9200:9200  -p 9300:9300 \n
    -e "discovery.type=single-node" \n 
    -e ES_JAVA_OPTS="-Xms84m -Xmx512m" \n 
    -v /home/xxx/elasticsearch/config/elasticsearch.yml:/usr/share/elasticsearch/config/elasticsearch.yml \n 
    -v /home/xxx/elasticsearch/data:/usr/share/elasticsearch/data \n 
    -v /home/xxx/elasticsearch/plugins:/usr/share/elasticsearch/plugins \n -d elasticsearch:7.14.2
```

