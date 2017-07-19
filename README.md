# mpi4py
### This quickstart aims to setup distributed system on raspberry pi and laptops. 

**denpendency**

install mpi4py on both laptop and raspberry pi

```
sudo apt-get install python-mpi4py
```

**setup passwordless ssh connection**

* check raspberry pi documentation for setting up [passwordless SSH connection](https://www.raspberrypi.org/documentation/remote-access/ssh/passwordless.md)

**create helloworld.py on remote machine**

```
hello world from pi
```

**store remote ip address on master machine**

```
echo 123.123.123.123 > ip
```

**execute command from master machine**

```
mpiexec -n 2 -machinefile ip python helloworld.py
```
