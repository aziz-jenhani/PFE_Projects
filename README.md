# React-Symfony-MySQL

## Requirements

1. Docker ( https://docs.docker.com/get-docker )

2. Docker Compose ( https://docs.docker.com/compose/install )

## How to run this stack ?

1. Clone the repository: 

  ``

2. We have two projects in this repository **backend** and **frontend**

3. Go to the cloned directory:

`$ cd `

4. Run the application:

`$ docker-compose up -d` 

5. Install Symfony Packages

`$ docker-compose run --rm backend composer install`

6. Apply Symfony migrations:

`$ docker-compose run --rm backend php bin/console doctrine:schema:create`

`$ docker-compose run --rm backend php bin/console hautelook:fixtures:load`

## URLs 

- Frontend-React: http://localhost:3101/ ( **Username: admin@localhost.io** / **Password: adminpass** )

- Backend-Symfony: http://localhost:8000/

- PhpMyAdmin: http://localhost:8011 ( **Login: root** / **Password: root** )


