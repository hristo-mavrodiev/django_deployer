# djangodeployer  
Deploy django project with nginx, gunicorn, supervisor, postgresql on debian.


### Quick start    
Creates the basic config file.  
``` bash
djangodeployer init
```
Edit the basic configuration dj_config.json.  
``` jsonc
{
    "IP_ADDRESS": "0.0.0.0",        # server public ip address
    "SERVER_NAME": "django-server", # hostname of the server
    "LINUX_USER": "dj",             # server username
    "DJ_PROJ": "djangosite",        # django project name
    "PG_USER": "djadmin",           # postgresql database username
    "PG_DB": "djangodb",            # postgresql database name
    "DOMAIN_NAME": "mywebsite.com"  # domain name
}
```
Deploy with the command:
``` bash
djangodeployer deploy
```


### License
MIT
