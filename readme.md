Nextcloud deployment via docker-compose

This project uses apache as the web server, mariadb as the database, and traefik for management of let's encrypt certificates. 
The traefik container is separated and can very easily be extended to provide traffic management to other docker-compose projects via networks (see network definitions in source)

This project requires split dns / host overrides for traefik to route traffic to the nextcloud and traefik dashboard services (as well as others should you care to extend it). 


known bugs: android/ios devices (app) hang on initial log in. This can be remedied with 'old login' option (if available) or app token.   