# Node Explorer

## Variables in ```settings.env```
##### VALIDATOR_ADDR - the public key of your validator
##### MASTER_SERVER_IP - IP address of the computer where Master Monitoring Server is installed

## Install software

### Update package repositories

```
sudo apt update
```

### Log in to ```kira``` user
```
sudo su - kira 
```
```
sudo -s
```

### Log in to the Kira Network Manager
```
kira
```

### Put the node in the maintenance mode
![Alt text](images/enable_maintaince.png?raw=true "Enable MAINTENANCE mode")

### Wait until the node changes its status to ```PAUSED```
![Alt text](images/paused_status.png?raw=true "Paused Status")


### Exit the Kira Network Manager by pressing the ```X``` key

### Clone the project and start installing
```
git clone https://github.com/SchlafenderFox/KiraNodeExplorer && cd ./KiraNodeExplorer && ./setup.sh
```

### Enter value for MASTER_SERVER_IP variable ```Example:```
![Alt text](images/enter_master_server_ip.png?raw=true "Paused Status")

### Reboot the server
```
reboot
```

### Log in to ```kira``` user
```
sudo su - kira 
```
```
sudo -s
```

### Log in to the Kira Network Manager
```
kira
```

### Restart all containers
![Alt text](images/restart_containers.png?raw=true "Restart all containers")

### Wait until the node is fully synchronized with the network.
![Alt text](images/full_sync.png?raw=true "Restart all containers")

### Exit the maintenance mode
![Alt text](images/disable_maintaince.png?raw=true "Disable MAINTENANCE mode")

### Wait until the node changes its status to ```ACTIVE```. It can take up to 1 hour, but in that time your node will be producing blocks.
![Alt text](images/active_status.png?raw=true "Active Status")