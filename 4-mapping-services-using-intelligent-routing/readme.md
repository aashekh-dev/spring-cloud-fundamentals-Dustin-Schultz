# mapping-services-using-intelligent-routing

Start the following services sequencewise

1) discovery-server
2) gateway-server
3) hello-service
4) goodbye-service

http://localhost:8761/

```
Application				AMIs		Availability Zones				Status
GATEWAY-SERVICE			n/a (1)	(1)	UP (1) - 					localhost:gateway-service
GOODBYE					n/a (1)	(1)	UP (1) - 					localhost:goodbye:2222
HELLO						n/a (1)	(1)	UP (1) - 					localhost:hello:1111
```

Now simply hit the ``http://localhost:8080/hello`` and you should be able to see

```
Hello from USA!
```