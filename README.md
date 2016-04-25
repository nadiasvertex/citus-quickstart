# citus-quickstart
Provides a vagrant file, an Ansible playbook, and a script that boots the cluster. A test database
called my_test is created for playing around.

To use, just run:

```bash
boot.sh
```

The cluster should provision itself with machine1 as the master and the rest workers.

The master node is machine1 (192.168.77.21). 

```bash
vagrant ssh machine1 -c "psql -u postgres -d my_test"
```

For more information you can read the manual here: https://www.citusdata.com/docs/citus/5.0/index.html

