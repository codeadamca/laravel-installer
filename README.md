# laravel-installer
A basic walk-through of setting up a new Laravel project.

There are two methods of setting up a new Laravel project: 

## Composer and Laravel

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

![MAMP Settings](https://raw.githubusercontent.com/codeadamca/laravel-installer/main/mamp-root-folder.png)

Once you have the Laravel installer installed, you will want to add it to your PATHS, so it is accessible from any folder using the command line. This is done slightly different on a Windows maching and a MAc:

### Windows

If you are using Windows, follow these steps:

1. Open up the Comman Prompt
2. Run the following commane: 
 
```
pathman /ru c:\Users\[Your User]\AppData\Roaming\Composer\vendor\bin
```

3. YOu can then run the command ```echo %PATH%``` to see a list of all current folders included.

### Mac

If you are using a Mac, follow these steps:

1. Open the Terminal
2. Open the paths file using VIM: 

```
sudo vim /etc/paths
```

3. Push the ```o``` key. This will insert a new line and change to insertion mode.
4. Add the path to the Laravel installer to your paths file:

```
/Users/Adam/.composer/vendor/bin
```

5. Push ```ESC```, this will exit insertion mode.
6. Type ```:wq```, this will save an exit.

## Create a New Laravel Project

You are now ready to create a new Laravel project. Open your command line tool, navigate to the folder you want to place the new project in, and then run the following command:

```
laravel new example-app
```
## Tutorial Requirements:

* [Visual Studio Code](https://code.visualstudio.com/)
* [Composer](https://getcomposer.org/) 
* [Laravel](https://laravel.com/)

Full tutorial URL: https://codeadam.ca/learning/laravel-installer

<a href="https://codeadam.ca">
<img src="https://codeadam.ca/images/code-block.png" width="100">
</a>
