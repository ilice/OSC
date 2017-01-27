# OSC

OSC application orchestration

[![Compose](https://www.docker.com/sites/default/files/Compose.png)](https://www.docker.com/products/docker-compose)

## Log management

[![2017-01-27_083558.png](https://s24.postimg.org/ie9aaon5h/2017_01_27_083558.png)](https://postimg.org/image/kvl1hy71t/)

## Load balancer

[![HAProxy](http://www.haproxy.org/img/logo-med.png)](http://www.haproxy.org/)

HAProxy provides us with round-robin load balancing, receives the web request and routes it to the web service.

We can scale the stack to 'n' web instances/containers conected to log manager. Then web request are received by the HAPoxy and routed ound-robin to all 'n' of the web instances. All these instances ar also linked to the log management system.

```
$ docker-compose scale web=3
```
