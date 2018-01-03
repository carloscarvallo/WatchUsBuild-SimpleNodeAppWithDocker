FROM postgres:9.6

LABEL maintainer carloscarvallo87@gmail.com 

EXPOSE 5432

COPY seed.sql /docker-entrypoint-initdb.d/
