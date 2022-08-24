# calysteau-laravel
A docker image with Apache, PHP, NodeJS and Laravel for dev

Based on SILARHI works (https://github.com/silarhi)

## Build it
```bash
docker build -t calysteau/calysteau-laravel .
```

# Run container
Run a new container with following parameters

   Container name : <CONTAINER-NAME>
   
   Ports : 80 - 80/tcp, 8000 - 8000/tcp
   
   Volumes : <HOST-DIR> - /app

## Create laravel app
From container CLI run 
```bash
laravel new <APP-NAME>
```

## Launch server

```bash
cd <APP-NAME>
php artisan serve --host 0.0.0.0
```

From host, access you laravel app on http://localhost:8000
