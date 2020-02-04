# How to install this web application Symfony V5.0.4 with PHP 7.3.5

## a) First Install Composer 
Please to refer to this link to install composer : https://getcomposer.org/
or skip it to the b), if it's already installed.

## b) Download all packages with Composer
To Launch all packages dependencies with this following command : 
`composer update`

## c) Configuration Vich/Uploader-bundle
Please to check this link, to configure the upload file location : https://github.com/dustin10/VichUploaderBundle/blob/master/docs/usage.md#step-1-configure-an-upload-mapping

## d) Configure .env
Please to copy and paste the ".end.dist" file with your configuration, and rename this one by ".env"
More information in this link : https://symfony.com/doc/current/configuration.html#configuring-environment-variables-in-env-files

/!\ You can use wamp to handle your database local : http://www.wampserver.com/ /!\

## e) Make Migration
After to configure your database (see the b) point, launch this command :
`php bin/console doctrine:migrations:migrate`
Then, you have to start this command :
`php bin/console doctrine:migrations:status`
To check the good version for this migration. We have to get this one value for "Current Version":
> Current Version: 2020-02-04 19:55:34 (20200204195534)

## f) Launch Symfony Server
Install Symfony, you have the documentation on this link : https://symfony.com/download
Then, you can start your local web server : 
`symfony server:start` after this, an local url will be generated.

## g) Create an Picture :
After to launch your web server, go to this url to create an new resource :
> your_local_url/picture/add

## h) Show an Picture :
When you web server is launched, go this url to see your resource :
> your_local_url/picture/id 
/!\ id is numeric value, which after exist after your create one. /!\

## i) List the Pictures :
When you web server is launched, go this url to see your resource :
> your_local_url/picture
