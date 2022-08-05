The focus will be mainly on what is used for gctools projects

 ## Docker


 ## Docker-compose


 ## on windows + WSL
 * on wsl and some other most restricted systems, you might not be able to use port 80, so a container will most likely run into errors trying to start and bind port 80
```yaml
ports:
    - 80:80
``` 
^
this will most likely cause the container to error and crash instantly, 

in this case try mapping to host a port like 8000 or any port over 1000 instead
```yaml
ports:
    - 8000:80
``` 
