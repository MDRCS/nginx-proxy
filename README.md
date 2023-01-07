# NGINX Proxy For A DJANGO REST API

## Usage

### Environment Variables

 - `LISTEN_PORT` - Port to listen on (default: `8000`)
 - `APP_HOST` - Hostname of the app to forward requests to (default: `app`)
 - `APP_PORT` - Port of the app to forward requests to (default: `9000`)


### Q&A

- why we didn't use standard nginx image and we used `nginxinc/nginx-unprivileged` ?
+ It's because nginx standard image use root user and it's not best practice          `nginxinc/nginx-unprivileged` use the least priveleged user.

- Alpine is the most light-weight image for any provider, and it's linux operating system that is designed for docker containers.