# gcp_instance_groups_demo - Startup Script for Load Balancer Test - HTTP. 

For USA 
```shell
#! /bin/bash

apk update

wget https://raw.githubusercontent.com/krausce/gcp_instance_groups_demo/main/frontend-uswest.py

python frontend-uswest.py &
```

For  Asia 

```shell
apk update

wget https://raw.githubusercontent.com/krausce/gcp_instance_groups_demo/main/frontend-asia.py

sudo python frontend-asia.py &
```


For  Europe 
```shell
#! /bin/bash

apk update

wget https://raw.githubusercontent.com/krausce/gcp_instance_groups_demo/main/frontend_europe.py

sudo python frontend_europe.py &
```

############################################################################


Curl Command

Slow 

while true ; do (curl http://[Load Balancer ExternalIP]/service ) ; sleep 2 ; done 


Fast

while true ; do (curl http://[Load Balancer ExternalIP]/service ) ; sleep 0.1 ; done 


