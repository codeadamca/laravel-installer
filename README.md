# laravel-installer
A basic walk-through of setting up a new Laravel project.

There are two methods of setting up a new Laravel project: 

## Compoaser and Laravel

You can use composer to simply download a new project scaffolding:

```
composer create-project laravel/laravel example-app
```

This is a simple method that only requires the installation of Composer. This command will work on both a Windows maching or a Mac.

## Laravel Installer

Or you can install the Laravel installer and use it to set up new Laravel scaffolding:

```
composer global require laravel/installer
laravel new example-app
cd example-app
php artisan serve
```

This will create a new Laravel application scaffolding in a folder names ```example-app``` and deploy the application using (Artisan)[https://laravel.com/docs/9.x/artisan#introduction] (the command line interface included with Laravel). 

You can also deploy the new Laravel application using a tool such as MAMP by pointing the root directory to ```example-app/public```.



### Windows

On a Windows maching you first need to install (Docker Desktop)[https://www.docker.com/products/docker-desktop]
