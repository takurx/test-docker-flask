# test-docker-flask
test, docker and flask and gunicorn and nginx

- Q2.
```
$ docker-compose build
ERROR: build path /home/ynakagawa/Works/test-docker-flask/web either does not exist, is not accessible, or is not a valid URL.
```

### A1.
- https://docs.docker.com/compose/install/
```
$ sudo curl -L "https://github.com/docker/compose/releases/download/1.29.1/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
[sudo] password for ynakagawa: 
  % Total    % Received % Xferd  Average Speed   Time    Time     Time  Current
                                 Dload  Upload   Total   Spent    Left  Speed
100   633    0   633    0     0   2388      0 --:--:-- --:--:-- --:--:--  2397
100 12.1M  100 12.1M    0     0  9857k      0  0:00:01  0:00:01 --:--:-- 13.8M
$ sudo chmod +x /usr/local/bin/docker-compose
$ sudo ln -s /usr/local/bin/docker-compose /usr/bin/docker-compose
$ docker-compose --version
docker-compose version 1.29.1, build c34c88b2
```

- Q1.
```
$ docker-compose build

Command 'docker-compose' not found, but can be installed with:

sudo snap install docker          # version 19.03.13, or
sudo apt  install docker-compose  # version 1.25.0-1

See 'snap info docker' for additional versions.
```