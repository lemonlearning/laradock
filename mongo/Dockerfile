FROM mongo:latest

MAINTAINER Mahmoud Zalt <mahmoud@zalt.me>

#COPY mongo.conf /usr/local/etc/mongo/mongo.conf

VOLUME /data/db /data/configdb

# Added by Adrian - restore the database from dump
# dump must be present in the mongo folder
COPY dump /dump
CMD mongorestore /dump

CMD ["mongod"]

EXPOSE 27017

