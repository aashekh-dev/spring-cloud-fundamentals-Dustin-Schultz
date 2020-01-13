# 05-calling-services-using-client-side-load-balancing

Make the following configurations for ``ribbon-time-service``, please make sure to select 
``com.example.RibbonTimeServiceApplication`` as main App.

![Alt text](images/ribbon-time-service-1.png?raw=true "Title")


![Alt text](images/ribbon-time-service-1.png?raw=true "Title")

Hit the ``http://localhost:4444/``

```
The current time is Sun Jan 12 21:43:36 IST 2020(answered by service running on 4444)
```

again hit the ``http://localhost:5555/`` 

```
The current time is Sun Jan 12 21:44:32 IST 2020(answered by service running on 5555)
```