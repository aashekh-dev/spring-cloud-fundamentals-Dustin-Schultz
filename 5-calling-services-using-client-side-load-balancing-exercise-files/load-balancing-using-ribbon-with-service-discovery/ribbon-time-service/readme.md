# 05-calling-services-using-client-side-load-balancing

Simply run the ``discovery-server`` and then make the following configurations for ``ribbon-time-service``, please make sure to select 
``com.example.RibbonTimeServiceApplication`` as main App.

![Alt text](images/ribbon-time-service-1.png?raw=true "Title")


![Alt text](images/ribbon-time-service-1.png?raw=true "Title")

Then simply run ``http://localhost:4444/`` 

```
The current time is Sun Jan 12 20:30:46 IST 2020(answered by service running on 4444)
```

Then simply run ``http://localhost:5555/`` 

```
The current time is Sun Jan 12 20:33:53 IST 2020(answered by service running on 5555)
```

Here you can see ``http://localhost:8761/`` services registered with eureka !!

and then start the "ribbon-time-service" and hit ``http://localhost:8080/``

```
The current time is Sun Jan 12 21:30:41 IST 2020(answered by service running on 4444)
```

again hit the same url

```
The current time is Sun Jan 12 21:31:48 IST 2020(answered by service running on 5555)
```