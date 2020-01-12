# config-server

http://localhost:8888/config-client-app/default

```
{
    "name": "config-client-app",
    "profiles": [
        "default"
    ],
    "label": null,
    "version": "1cb37c9ba1fa4c17d2ae7489c2e592eba1688547",
    "state": null,
    "propertySources": [
        {
            "name": "https://github.com/dustinschultz/scf-config-repository/config-client-app.properties",
            "source": {
                "some.property": "app specific overridden value"
            }
        },
        {
            "name": "https://github.com/dustinschultz/scf-config-repository/application.properties",
            "source": {
                "some.property": "global",
                "some.other.property": "global"
            }
        }
    ]
}
```

http://localhost:8888/config-client-app/prod

```
{
    "name": "config-client-app",
    "profiles": [
        "prod"
    ],
    "label": null,
    "version": "1cb37c9ba1fa4c17d2ae7489c2e592eba1688547",
    "state": null,
    "propertySources": [
        {
            "name": "https://github.com/dustinschultz/scf-config-repository/config-client-app-prod.properties",
            "source": {
                "some.property": "profile specific value",
                "some.other.property": "profile specific value"
            }
        },
        {
            "name": "https://github.com/dustinschultz/scf-config-repository/config-client-app.properties",
            "source": {
                "some.property": "app specific overridden value"
            }
        },
        {
            "name": "https://github.com/dustinschultz/scf-config-repository/application.properties",
            "source": {
                "some.property": "global",
                "some.other.property": "global"
            }
        }
    ]
}
```


http://localhost:8888/config-client-app.properties

```
some.other.property: global
some.property: app specific overridden value
```

http://localhost:8888/config-client-app.yml

```
some:
  other:
    property: global
  property: app specific overridden value
```


