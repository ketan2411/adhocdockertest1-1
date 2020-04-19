# adhocdockertest1
task1:

#created a dockerfile for image
FROM alpine
MAINTAINER singhvikajal258@gmail.com
CMD date +%H:%M:%S >> time.txt

#created an image 
docker build -t kajal:v1

#container started
docker start -i kajal

task 4:
Question4
FROM centos
RUN yum install httpd
RUN mkdir /webapp1
COPY webapp /webapp1
EXPOSE 80
ENTRYPOINT httpd -DFOREGROUND

docker build -t kajal:q4 .

