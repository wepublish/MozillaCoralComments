# MozillaCoralComments
Docker Compose for Mozilla Coral Project used for Comments

Bootup a Container-Optimized OS on Google VM 

Download and run the Docker Compose image. Check the tags for Docker Compose to use the latest version.
$ docker run docker/compose:1.23.2 version

Clone the Standart docker-compose.yml and config password and ip
$ git clone https://github.com/wepublish/MozillaCoralComments.git

Change Directory to the git Dir and run the Service
$ docker run --rm \
    -v /var/run/docker.sock:/var/run/docker.sock \
    -v "$PWD:/rootfs/$PWD" \
    -w="/rootfs/$PWD" \
    docker/compose:1.13.0 up 

Login on the Admin Panel yay !
http://yourIP:3000/admin/install 

For further Instructions rtfm : https://docs.coralproject.net/talk/#setup
