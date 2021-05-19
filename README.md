Ansible (ETCD)

Prerequisites 
---
CentOS8


Usage
---

Test connection  ```ansible etcd -i environment/default/ -m ping```

Run ```ansible-playbook -i environment/default/ playbook.yml```


Testing
---

```./etcdctl --endpoints=https://192.168.122.13:2379 --cacert=/etc/etcd_certs/ca.pem --cert=/etc/etcd_certs/node.pem --key=/etc/etcd_certs/node-key.pem endpoint  status -w table```
