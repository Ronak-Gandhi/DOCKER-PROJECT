# DOCKER-PROJECT

## I have completed my Docker Project under the guidance of Vimal Daga sir under IIEC RISE Campaign..
So i have created whole setup which launches JOOMLA (which is a free and open-source content management system (CMS) for publishing web content), by using DOCKER COMPOSE (which provides a way to orchestrate multiple containers that work together)..
 
 _I installed docker on the top of RHEL8(redhat enterprise linux) and then disabled firewall security ,after that downloaded MySQL:5.7  and joomla:3.9-php7.2-apache IMAGES..also Docker Hub allows us to even share our own images and i used built-in images for MySQL and for JOOMLA..then created a YAML file as docker-compose.yml in which the piece of code launch two services,one for joomlaos and another for database names dbos..and depends_on expresses dependencies between services..and To Expose our container we require ports which defines that docker shall re-route the port 80 from the application to the port 8083 of hosting machine. with ports you open the connections via that port for all machines and Volumes is mounting one route from the hosting machine to the route specified into the container and mysql & joomla stores their data inside some folders and made them permanent by mounting those volumes,so that if container terminates ,our data wont lost..and many images in docker requires pre-defined environment variables to run,so that environment created..and then by docker-compose up -d , the joomla php/apache server fired up on one click and here -d means it runs in background..and then run docker ls command to see them listed..and find IP address of joomla image by docker inspect command and on rhel8 browser,inserted that IP with port number and then JOOMLAA website opened..we can also stop the whole setup by docker-compose stop command and can restart is by docker-compose start command_...
 
# All the screenshots of whole process is in another folder, named Docker Project.docx and yml file is on docker-compose.yml !! 

## THANKYOU!!
