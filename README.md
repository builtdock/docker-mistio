docker-mistio
=============

```

## for the impatient // one command setup :)
docker run -td -p 8000:8000 docker-mistio

## thats it
visit http://[server/host ip]:8000

```

```
## to build the image / slower way but you can now customize 
git clone https://github.com/builtdock/docker-mistio.git 
cd docker-mist
docker build -t mistio .
docker run -td -p 8000:8000 mistio 
```
#### http://[server/host ip]:8000 

Please note this has no login/authentication whatever for now. Please use it only on internal network 

Or use an Nginx proxy or some other auth mechanism if you prefer to use it in production which may not be advised at the moment.

This code ONLY allows you to manage inventory /shell commands but does not have monitoring features and require login to http://mist.io for some reason. 

### if youd like develop/contribute you may need a shell please use the following command and cd /home/mist 
```
docker run -ti -p 8000:8000 mistio /bin/bash
```


### Credits/ More info

https://github.com/mistio/mist.io


