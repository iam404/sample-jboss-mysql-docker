# sample-jboss-mysql-docker
###Step 1: Build Mysql Image###

 docker build -f Dockerfile-mysql -t sample/mysql .
 
###Step 2: Build Jboss Image with .war file on directory###

 docker build -f Dockerfile-jboss -t sample/jboss .
 
###Step 3: Create a container with Jboss & Mysql linked###
 
 docker-compose up -d
