## cryptsetup_remote_unlock

[![Travis CI](http://img.shields.io/travis/ypid/ansible-cryptsetup_remote_unlock.svg?style=flat)](http://travis-ci.org/ypid/ansible-cryptsetup_remote_unlock)


Configure an encrypted headless system to get the password over SSH.

See http://unix.stackexchange.com/a/79203




### Role variables

List of default variables available in the inventory:

    ---
    
    cryptsetup_remote_unlock_local_ssh_dir: "/root/.ssh"
    cryptsetup_remote_unlock_remote_ssh_dir: "/etc/initramfs-tools/root/.ssh"
    cryptsetup_remote_unlock_public_key: ""
    
    # cryptsetup_remote_network_interface: "eth0"
    cryptsetup_remote_network_ip_line: "{{ ansible_eth0.ipv4.address }}:::{{ ansible_eth0.ipv4.netmask }}:{{ ansible_hostname }}::off"
    # cryptsetup_remote_network_ip_line: "192.0.2.23:::255.255.255.0:noname::off"
    # ip=<client-ip>:<server-ip>:<gw-ip>:<netmask>:<hostname>:<device>:<autoconf>
    # https://www.kernel.org/doc/Documentation/filesystems/nfs/nfsroot.txt




### Authors and license

`cryptsetup_remote_unlock` role was written by:

- [Robin Schneider](https://github.com/ypid) | [e-mail](mailto:ypid@riseup.net)

License: [AGPLv3](https://tldrlegal.com/license/gnu-affero-general-public-license-v3-%28agpl-3.0%29)

***

README generated by [Ansigenome](https://github.com/nickjj/ansigenome/).
