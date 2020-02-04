# How to install this web application 
## a) First Install Composer 
Please to refer to this link to install composer : https://getcomposer.org/
or skip it to the b), if it's already installed.

## b) Configure .env
Please to copy and paste the ".end.dist" file with your configuration, and rename this one by ".env"
More information in this link : https://symfony.com/doc/current/configuration.html#configuring-environment-variables-in-env-files

## c) Download all packages with Composer
To Launch all packages dependencies with this following command : 
`composer update`

## d) Make Migration
After to configure your database (see the b) point, launch this command :
`php bin/console doctrine:migrations:migrate`
Then, you have to start this command :
`php bin/console doctrine:migrations:status`
To check the good version for this migration. We have to get this one value for "Current Version":
> Current Version: 2020-02-04 19:55:34 (20200204195534)
