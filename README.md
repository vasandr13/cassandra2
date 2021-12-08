# Ansible Role for Installing and Configuring Apache Cassandra Cluster.

# Prerequisites:
RedHat based OS.

Ansible Version >= 2.9

This one works fine:
https://hub.docker.com/r/willhallonline/ansible

Java (JDK) >= 8

How to run:

```shell
git clone https://github.com/vasandr13/cassandra.git;
```


```shell
sudo docker pull willhallonline/ansible;
```

```shell
sudo docker run --rm -it --entrypoint="" \
                -v ${HOME}/ansible:/root/ansible:ro \
                --name ${LOGNAME}_ansible \
                willhallonline/ansible:2.9 \
                ansible-playbook -i inventory.ini playbooks/cassandra.yml;
```



# All kudos goes to:

https://github.com/locp/ansible-role-cassandra

https://galaxy.ansible.com/locp/cassandra

