Nextcloud deployment via docker-compose

This project creates a nextcloud instance via docker. It uses apache as the web server, mariadb as the database, and traefik for management of let's encrypt certificates. 
The traefik container is separated and can very easily be extended to provide traffic management to other docker-compose projects via networks (see network definitions in source)

known bugs: android/ios devices (app) hang on initial log in. This can be remedied with 'old login' option (if available) or app token.   