# Infra-Scripts
Some handy initctl scripts

## Usage

1. in /etc/init add
  - flower-server-service.conf
  - abc_backend_service.conf
  - redis-server-service.conf
1. in /etc/init.d add
  - celeryd
1. in /etc/default add
  - celeryd

### Gunicorn server
```
sudo initctl start abc_backend_service
```

### Celery
```
sudo service celeryd start
```

### Redis
```
sudo initctl start redis-server-service
```

### Flower
```
sudo initctl start flower-server-service 
```
