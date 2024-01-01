docker exec -it demo-postgres-14.2 /bin/bash

<!-- Para ingresar al bash del contenedor de Rails que está saliendo con el código 0, puedes usar el siguiente comando: -->
ejecuta el contenedor en otra imagen
  - docker-compose run demo-web /bin/bash

ejecuta el contenedor en la misma imagen
  - docker-compose exec demo-web /bin/bash

docker exec -it demo-postgres-14.2 psql --username=jic  --dbname=post_production

CREATE USER postgres WITH PASSWORD 'This_is_a_secure_password';
ALTER USER postgres WITH SUPERUSER;
select * from pg_user;

