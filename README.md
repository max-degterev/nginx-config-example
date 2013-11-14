# MP.nginx-node

This is helpful for running multiple [MP.boilerplate](https://github.com/moviepilot/mp.boilerplate) apps alongside.

## Usage:
### Downloading and updating
  1. Install nginx:

    `brew install nginx`

  2. Swap your nginx config with one from the repo

    `sudo rm -f /usr/local/etc/nginx/nginx.conf`
    `ln -s ~/Projects/mp.nginx/nginx.conf /usr/local/etc/nginx/nginx.conf`

    where ~/Projects/mp.nginx/nginx.conf is your _MP.nginx-node_ location

### Start

  `nginx`

  Server will be running on port 3000 by default. Make sure that port is free.

### Stop

  `nginx -s stop`

### Restart

  `nginx -s stop && nginx`
