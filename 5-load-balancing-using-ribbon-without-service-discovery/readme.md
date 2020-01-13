# load-balancing-using-ribbon-with-service-discovery

Simply maintain two configurations while running the ribbon-time-service.

Make sure to start on `4444` and `5555` port, set the respective configurations for the same.

Now start the ribbon-time-app and then simply hit the `http://localhost:8080/`

```
The current time is Mon Jan 13 11:57:59 IST 2020(answered by service running on 5555)
```

and one more refresh 

```
The current time is Mon Jan 13 12:01:05 IST 2020(answered by service running on 4444)
```