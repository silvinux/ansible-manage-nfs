# README.md
# Ansible Role: manage-nfs 1.0

This role is able to mount/umount and/or add/remove/modify permission on a nfs share, using booleans to activate/deactivate functions.

## Requirements

This role requires Ansible 1.9 or higher, and platform requirements are listed in the metadata file.

## Role Variables

Available variables are listed below, along with default values:

## Activate/deactivate functions
--- 
	ShareState: "mounted"	||   "unmounted" || "absent"
	manage: false
	permissions: false

### NFS Parameters
	nfsopts: "defaults,_netdev,tcp,nfsvers=3"
	nfsopts_rman: "rw,_netdev,bg,exec,hard,nointr,rsize=32768,wsize=32768,tcp,actimeo=0,vers=3,timeo=600"

## Dependencies
There is no dependencies with other roles.

## Examples Playbook
1. Mount NFS share.

## License
GPLv3
