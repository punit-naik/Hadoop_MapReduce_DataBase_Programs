Hadoop_MapReduce_DataBase
=========================

This repository contains the source code of a WordCount program which writes its output to the MySQL database.
If you are writing to a remote database (i.e. if you are running this program on a multinode cluster), make sure that the bind address in the file "/etc/mysql/my.cnf" is the IP address of the Master nodeand also in the driver class of the hadoop mapreduce program, make sure that the DB URL contains either the hostname or the IP address of the Master node.
Also make sure that MySQL Server, MySQL Client and libmysql-java is installed on all the nodes.
If you are running this code on a single node cluster, the bind address and the DB URL should contain localhost.
