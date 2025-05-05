<p align="center">
    <h1 align="center" style="color:skyblue">Wholesaling</h1>
    <p align="center">
        <img src="https://img.shields.io/badge/Laravel-12.0-red?logo=laravel">
        <img src="https://img.shields.io/badge/PHP-8.2-violet?logo=php">
        <img src="https://img.shields.io/badge/React.js-18.2-skyblue?logo=react">
        <img src="https://img.shields.io/badge/TypeScript-5.0.2-yellow?logo=typescript">
        <img src="https://img.shields.io/badge/Inertia.js-2.0.0-magenta?logo=inertia">
        <img src="https://img.shields.io/badge/MUI-6.4.7-magenta?logo=mui">
    </p>
</p>


## About
<p style="text-indent: 0.5em">
This web app is a wholesaling management system developed with Laravel and React.js using Inertia.js and Material UI.
</p>

## How to run this web app

1. create docker container
    
    (below is an example code)
    ```bash
    docker create --name [mycontainer] -it -p 8000:8000 -p 5173:5173 -v /path/to/repos/parent/folder/in/local/:/home/[username]/parent/folder/pathname/ ubuntu:latest
    ```

1. start and attach the created docker container
    ```bash
    docker start [mycontainer] && docker attach [mycontainer]
    ```
1. update apt
    ```bash
    apt update
    ```
1. install necessary packages for the app
    ```bash
    apt-get install -y git php mariadb-server and so on ...
    ```

1. install composer and set configuration 
    
    follow the installation instruction of composer at its webpage.   

1. git configuration
    ```bash
    git config --global user.name [github_username]

    git config --global user.email [github_username@users.noreply.github.com]
    ```
1. clone the repository
    ```bash
    git clone https://github.com/ken-script/wholesaling.git wholesaling
    ```

1. move inside the repository workspace
    ```bash
    cd wholesaling
    ```

1. install necessary libraries for the app
    ```bash
    composer install
    ```
    if some errors occur when installing composer packages then install the lacked packages.

1. copy .env.example file to 
    ```bash
    cp .env.example .env
    ```

1. generate key
    ```bash
    php artisan key:generate
    ```

1. set up MariaDB
    ```bash
    mysql_secure_installation
    ```

1. run MariaDB
    ```bash
    service mariadb start
    ```

1. DB migration
    ```bash
    php artisan migrate
    ```

1. run the app
    ```bash
    php artisan serve
    ```

1. access the web app in the browser running on `localhost:8000`


## License
<p style="text-indent: 0.5em">
Apache 2.0
</p>