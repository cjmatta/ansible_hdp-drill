### Install Drill on HDP

This is an ansible playbook to install [Apache Drill](http://drill.apache.org) on [Hortonworks Data Platform](http://hortonworks.com)

Example run:

```
ansible-playbook -i ~/cluster/hdp -u centos -b install_drill.yml
```

Example Inventory file:

```
[cluster]
ip-172-16-1-202.ec2.internal
ip-172-16-1-203.ec2.internal
ip-172-16-1-204.ec2.internal

[zookeeper]
ip-172-16-1-202.ec2.internal
ip-172-16-1-203.ec2.internal
ip-172-16-1-204.ec2.internal

[hiveserver]
ip-172-16-1-203.ec2.internal

[namenode]
ip-172-16-1-202.ec2.internal
```
