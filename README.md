## Please change SSH path in Vagrantfile to yours with your own image or read the following instructions.

  - Download image with certificate which, are placed in in ssh-keys folder from [link](https://goo.gl/Oam3Ln).
  - Put this certificates to your "~/.ssh" folder.
  - Add new box file with "ub14x64" name to your box list. 
```sh
$ vagrant box add ub14x64 ub14x64.box
```
  - Then start our machines.
```sh
$ vagrant up
```
  - At the end send request to the load balancer IP address.
```sh
$ curl http://192.168.120.122
<h1 style='color:blue'>Hello Datanyze!</h1>
```
