## Web push notifications channel for Laravel

A basic example of using webpush notifications with laravel and Javascript. Push Notifications are a part of Service Workers and It requires HTTPS unless you are using localhost.

#### Running this web application

-make sure you have xampp or wamp installed if you are on windows machine, mamp for mac , and lamp for linux.

-clone this repository to your local machine or just download the zip.

-install Composer first, then run this command in your command-line (you should be inside your project directory).

  `composer install`
-rename .env.example to .env and configure your database.

-generate application key.

    `php artisan key:generate`
-create tables by migrations.

    `php artisan migrate`
    
-Generate VAPID Keys (this command will place the VAPID keys in your .env file).

    `php artisan webpush:vapid`
    
-Add the VAPID public key to application server key in enable-push.js file located in public/js directory, here's the link to that line.

Run `npm install` and `npm run build`.

-Start Laravel dev server.

    `php artisan serve`

Read the entire tutorial Push Notifications with Laravel and Webpush on Medium.

Webpush package is used by this app.
