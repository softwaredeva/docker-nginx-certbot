# Boilerplate for nginx with certbot on docker-compose

`init-certbot.sh` fetches and ensures the renewal of a Let’s
Encrypt certificate for one or multiple domains in a docker-compose
setup with nginx.
This is useful when you need to set up nginx as a reverse proxy for an
application.

## Installation
1. [Install docker-compose](https://docs.docker.com/compose/install/#install-compose).

2. Clone this repository: `git clone https://github.com/softwaredeva/docker-nginx-certbot.git .`

3. Modify configuration:
- Add domains and email addresses to init-certbot.sh
- Modify configuration files in 'nginxconf'

4. Run the init script:

        ./init-certbot.sh

5. Create 'docker-compose.override.yml' file if needed:

6. Run the server:

        docker-compose up

## License
All code in this repository is licensed under the terms of the `MIT License`. For further information please refer to the `LICENSE` file.

Inpired from:
https://github.com/nnd/nginx-certbot/blob/master/init-certbot.sh
https://medium.com/@pentacent/nginx-and-lets-encrypt-with-docker-in-less-than-5-minutes-b4b8a60d3a71
https://stackoverflow.com/questions/38088279/communication-between-multiple-docker-compose-projects