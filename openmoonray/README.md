## How to install MoonRay on Rocky Linux  
  
### Start with a fresh Rocky 9.1 minimal install system   
```
dnf install -y epel-release
```  
```
dnf install -y ansible wget
```  
```
wget https://raw.githubusercontent.com/cyburdine/how-to/main/openmoonray/openmoonray-rocky9-base.yml
```  
```
wget https://raw.githubusercontent.com/cyburdine/how-to/main/openmoonray/openmoonray-rocky9-depbuild.yml
```  
```
wget https://raw.githubusercontent.com/cyburdine/how-to/main/openmoonray/openmoonray-rocky9-build.yml
```  
```
ansible-playbook openmoonray-rocky9-base.yml
```  
```
ansible-playbook openmoonray-rocky9-depbuild.yml
```  
```
ansible-playbook openmoonray-rocky9-build.yml
``` 
