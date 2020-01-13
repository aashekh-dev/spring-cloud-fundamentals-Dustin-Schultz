# configuring-services-using-distributed-configuration

Simply start discovery-server and then config-server and then config-app-client ``http://localhost:8761/``

You should be able to see

```
CONFIG-CLIENT-APP
```

then hit ``http://localhost:8080/`` then

```
app specific overridden value || global
```

POST ``http://localhost:8080/refresh``

This will give the list of the property fields that has been changed !!