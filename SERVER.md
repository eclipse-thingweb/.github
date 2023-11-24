# Eclipse Server Information

## Redirects

The current redirects in place are:

```
<VirtualHost *:80>
    ServerName plugfest.thingweb.io
    RedirectPermanent /playground-new https://playground.thingweb.io
    RedirectPermanent /index.html https://www.thingweb.io/services
</VirtualHost>
```

## Ports Documentation

Eclipse Thingweb uses a cloud instance provided by Eclipse Foundation to host its services on [plugfest.thingweb.io](http://plugfest.thingweb.io/). 
In order to function as a TCP/UDP server, we have some ports open to the public Internet.
These are documented below, alongside the service using the port.

### TCP Ports

| TCP PORT | Service |
|----------|---------|
|   80     |  Apache Web Server |
|   8080   |  -       |
|   8081   |  -       |
|   8082   |  -        |
|   8083   |  Example Things (HTTP) |
|   8084   |  -       |
|   8085   |  -       |
|   8086   |  -       |
|   8087   |  -       |
|   8088   |  WoT FX UI |
|   8089   |  -       |
|   5685   |  -       |


### UDP Ports

| UDP PORT | Service |
|----------|---------|
|   5680   |  -       |
|   5681   |  -       |
|   5682   |  -       |
|   5683   |  Example Things (CoAP) |
|   5684   |  -       |
|   5686   |  -       |
|   5687   |  -       |
|   5688   |  -       |
|   5689   |  -       |
