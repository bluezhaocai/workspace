# some operation instructions on MAC OSX

1. How to create share path by nfs server

>. configure nfs share path in /etc/exports. If the file is not exist, please create it

    `/home/tmp -maproot=root:wheel -network 192.168.56.0 -mask 255.255.255.0`

>. excute nfs commands to start nfs service

    sudo nfsd enable
    sudo nfsd start

>. show the mount point

    showmount
    Hosts on localhost:
    192.168.100.164