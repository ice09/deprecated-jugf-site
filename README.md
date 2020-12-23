# JUGF Community Site Creation

## Prerequisites

* Install Hugo
* Install Ananke

## Automatic Deployment on Change

* Git clone recursive for submodules

`git clone --recursive https://github.com/ice09/jugf-site.git`

* Add Cronjob for automated git pull with `crontab -e`

`
*/1 * * * * cd /jugf/site/checkout/jugf-site && git reset --hard origin/main && git fetch origin
`

## Start Hugo Static Website Creation & Hosting

`docker-compose up`

## Access Generated Pages

`http://${URL}` or `http://${URL}:1313`