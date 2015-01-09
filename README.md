# docker-phpLDAPadmin

A docker image to run phpLDAPadmin

## Quick start

### Get phpLDAPadmin in 1''
Run docker container with your custom environment variables :

    sudo docker.io run -p 443:443 \
               -e LDAP_HOST=ldap.example.com \
               -e LDAP_BASE_DN=dc=example,dc=com \
               -e LDAP_LOGIN_DN=cn=admin,dc=example,dc=com \
               -d osixia/phpldapadmin

phpLDAPadmin should be running on https://localhost

If you do not want SSL, set env NOSSL=1. Otherwise, all http traffic will be redirected to https. This is added for installations where the container is running in mesos, or some other environment where ssl is offloaded at the load-balancer.

### Whant more ? Openldap & phpLDAPadmin in 2''

to be completed :)


## Available Configuration Parameters

## Examples

### Customise self signed certificate

### Use your own ssl certificate

### Get phpLDAPadmin using TLS


## Do it yourself

### Build image

Clone the repository

    git clone https://github.com/osixia/docker-phpLDAPadmin
    cd docker-phpLDAPadmin

Build image

    sudo docker.io build -t phpldapadmin .

