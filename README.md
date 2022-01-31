# Quick reference

-	**Maintained by**:  
	[MariaDB developer community](https://github.com/MariaDB/mariadb-docker)

-	**Where to get help**:  
	[Database Adminstrators (Stack Exchange)](https://dba.stackexchange.com/questions/tagged/docker+mariadb), [MariaDB Knowledge Base](https://mariadb.com/kb/en/docker-and-mariadb/) ([Ask a Question here](https://mariadb.com/kb/en/docker-and-mariadb/ask) available).

Also see the ["Getting Help with MariaDB" article on the MariaDB Knowledge Base](https://mariadb.com/kb/en/getting-help-with-mariadb/).

# Supported tags and respective `Docker compose file` links

-	[`10.7`](https://github.com/deck-app/mariadb/blob/master/docker-compose.yml)
-	[`10.6`](https://github.com/deck-app/mariadb/blob/master/docker-compose.yml)
-	[`10.5`](https://github.com/deck-app/mariadb/blob/master/docker-compose.yml)

# Quick reference (cont.)

-	**Where to file issues**:  
	Issues can be filed on [https://github.com/deck-app/](https://github.com/deck-app/mariadb/issues) "Docker compose" Component, or on [GitHub](https://github.com/deck-app/mariadb/issues)

-	**Supported architectures**: ([more info](https://github.com/docker-library/official-images#architectures-other-than-amd64))  
	[`amd64`](https://hub.docker.com/r/amd64/mariadb/), [`arm64v8`](https://hub.docker.com/r/arm64v8/mariadb/), [`ppc64le`](https://hub.docker.com/r/ppc64le/mariadb/), [`s390x`](https://hub.docker.com/r/s390x/mariadb/)


# What is MariaDB?

MariaDB Server is one of the most popular database servers in the world. It’s made by the original developers of MySQL and guaranteed to stay open source. Notable users include Wikipedia, DBS Bank, and ServiceNow.

The intent is also to maintain high compatibility with MySQL, ensuring a library binary equivalency and exact matching with MySQL APIs and commands. MariaDB developers continue to develop new features and improve performance to better serve its users.

![logo](https://raw.githubusercontent.com/docker-library/docs/fe985dcb24154456254e252d1fa4a2b6b656ee80/mariadb/logo.png)

# How to use this image

## Start a `mariadb` server instance using DECK

Install MariaDB from the DECK marketplace and follow the instructions on the GUI

## Connect to MariaDB from the MySQL/MariaDB command line client

The following command starts another `mariadb` container instance and runs the `mysql` command line client against your original `mariadb` container, allowing you to execute SQL statements against your database instance:

```console
$ mysql -h mariadb_hostname -u example-user -p
MariaDB [(none)]> SELECT VERSION();
```

## From terminal with Docker
```console
$ git clone https://github.com/deck-app/mariadb.git
$ cd mariadb
$ docker-compose up -d

```
### Edit `.env` file to change any settings before installing like mariadb versions
```console
docker-compose up -d
```
### Modifying project settings
From the DECK app, go to stack list and click on `project's More > configure > Advanced configuration` Follow the instructions below and restart your stack from the GUI