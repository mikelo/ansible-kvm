# nice little KVM provisioning bundle using ansible

heavily inspired from https://www.redhat.com/sysadmin/build-VM-fast-ansible

to provision and run the VM:

```
ansible-playbook -K kvm_provision.yaml
```

find the IP address of the machine

```
sudo virsh domifaddr f36-lab01
Name       MAC address          Protocol     Address
-------------------------------------------------------------------------------
vnet2      52:54:00:5a:5f:3c    ipv4         192.168.122.170/24
```
access the virtual machine using ssh:
```
ssh root@192.168.122.170
```