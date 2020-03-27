FROM mysql:5.7

ENV MYSQL_ROOT_PASSWORD "dac"

ENV MYSQL_DATABASE "springrestdb"

# ENV MYSQL_USER "newdac"
# 
# ENV MYSQL_PASSWORD "dac"
# 
# ENV MYSQL_ROOT_HOST=%

COPY ./schema.sql /docker-entrypoint-initdb.d


EXPOSE 3306

# COPY wait-for-it.sh /wait-for-it.sh

# RUN chmod +x /wait-for-it.sh
