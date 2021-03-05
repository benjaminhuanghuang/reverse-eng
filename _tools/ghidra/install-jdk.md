
## Linux / apt / openJDK
```
  # update the apt package index
  sudo apt update  

  # install the default Java OpenJDK package
  sudo apt install default-jdk
```




## Env variable
edit ~/.bashrc  or ~/zshrc
``` 
  export JAVA_HOME=""
  export PATH=$PAHT:${JAVA_HOME}/bin
```