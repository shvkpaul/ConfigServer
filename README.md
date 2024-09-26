# ConfigServer


# DB CREATION
create database productdb;

create user 'product-team'@'%' identified by 'product-team-pass';

create user 'product-team'@'localhost' identified by 'product-team-pass';

grant all on *.* to 'product-team'@'%' with grant option;

flush privileges;

# Zipkin
http://localhost:9411/zipkin/

# Kafka Topic
http://localhost:8085/ui/docker-kafka-server/topic

# Redis data
http://localhost:8086