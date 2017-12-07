server:

mysql -u root -p

create database testdb;

quit

gcc userdb.c -o userdb

./userdb

gcc server.c -o server mysql_config --cflags --libs

./server

client:

gcc client.c -o client

./client
