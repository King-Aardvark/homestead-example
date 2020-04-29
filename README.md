#Intro
This is an example of using Laravel Homestead on a per project installation using composer. 

# Prerequisites
Before launching your Homestead environment, you must install 
`Vagrant` and at least one virtual machine provider `VirtualBox 6.x, VMWare, Parallels or Hyper-V`.
 All of these software packages provide easy-to-use visual installers for all popular operating systems.
 
To use the VMware provider, you will need to purchase both VMware Fusion / Workstation and the VMware Vagrant plug-in.
 Though it is not free, VMware can provide faster shared folder performance out of the box.
   
To use the Parallels provider, you will need to install Parallels Vagrant plug-in. It is free of charge.

# Running Homestead Example
```
git clone https://github.com/King-Aardvark/homestead-example.git
cp .env.example .env
composer install
php vendor/bin/homestead make (Creates Homestead.yaml. Can be used to change VM provisions)
vagrant up
yarn install (npm is another option)
yarn run development
```
For hostname resolution to work you need to add the default vm ip `192.168.10.15` to your `/etc/hosts` file.

#Further Reading
[Homestead Docs](https://laravel.com/docs/master/homestead)
