This nginx repo is part my docker deploy script [here](https://github.com/Jayzz55/docker-deploy-script)

This nginx repo is used to push the nginx config setting to the targetted server.

Example to add git remote server on staging:
`git remote add staging ssh://vagrant@127.0.0.1:/var/git/nginx.git`

Part of this deployment strategy is to use NGINX in the forefront to do reverse proxy with following ports:
* port 80 / 443 - rails app (port 3000)
* port 5000 - cadvisor (port 8080)
* port 5001 - kibana (port 5601)

