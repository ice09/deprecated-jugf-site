# JUGF Community Site Creation

## Prerequisites

* Install Hugo
* Install Ananke

## Automatic Deployment on Change

* Add Cronjob for automated git pull

```
*/1 * * * * cd /jugf/site/checkout/jugf-site && git reset --hard origin/main && git fetch origin
```

## Start Hugo Static Website Creation & Hosting

`docker-compose up`

## Access Generated Pages

`http://${URL}` or `http://${URL}:1313`