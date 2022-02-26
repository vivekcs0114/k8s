## ping setup

### Prerequisite
1. ingress

Please make sure all the above services are up and running.

### Install ping

```
helm upgrade --install ping .
```

### Check the container logs or check the link to make sure application is running 

```http://localhost/ping/```

#### Note: replace the localhost with the host that you have confirure in ingress