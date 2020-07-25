# symfony-elasticsearch

Simple elastic search developed with symfony searching in article entity by docker

After download poroject run following commands;

composer install

php bin/console doctirne:database:create

php bin/console doctrine:schema:update --force

docker-compose -f docker-compose.yaml up -d

php bin/console fos:elastica:create

"Add some data to article entity for search"

php bin/console fos:elastica:populate

symfony serve -d
