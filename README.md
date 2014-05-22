# NGINX-config-example

This is helpful for running multiple apps alongside.
Short intro on how to use and configure nginx for beginners: http://learnaholic.me/2012/10/10/installing-nginx-in-mac-os-x-mountain-lion/

Nginx documentation: http://wiki.nginx.org/Main
Location rules: http://wiki.nginx.org/HttpCoreModule#location

## Setup:

  1. Install nginx:

    `brew install nginx`

  2. Swap your nginx config with one from the repo

    `sudo rm -f /usr/local/etc/nginx/nginx.conf`
    `ln -s $(pwd)/nginx.conf /usr/local/etc/nginx/nginx.conf`

    where `$(pwd)/nginx.conf` is your NGINX-config-example location.

  3. Update nginx.conf `$repo_root` to point to your NGINX-config-example location

  4. Party hard

     ![Communism: it's a party](http://voicesofthenation.com/wp-content/uploads/2011/12/communism.jpg)

## Start:

  `nginx`

  Server will be running on port 3000 by default. Make sure that port is free.

## Stop:

  `nginx -s stop`

## Restart:

  `nginx -s stop && nginx`
