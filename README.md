# Ender's etcd

etcd Ansible Role

Setup local testing environment quickly and easily.

# Features

- \[DOING\] etcd Cluster

# Common Variables

## Common Variables

- `etcd_version`, etcd version, default is `v3.5.7`
- `etcd_home`, etcd home directory, default is `/opt/etcd`
- `etcd_ip_address`, **REQUIRD**, node external ip address
- `etcd_data_dir`, etcd data directory, default is `/data/etcd/data`
- `etcd_wal_dir`, etcd WAL directory, default is `/data/etcd/wal`

# Demo

Setup the VMs:

```
vagrant up
```

Deploy:

```
ansible-playbook deploy.yml
```
