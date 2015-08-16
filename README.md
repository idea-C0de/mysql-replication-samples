## mysql-replication-samples
A collection of tools for deploying and testing replication topologies with MySQL and MariaDB

The files in this collection are here to help beginners who want to start using advanced features like multi-source replication and test how they work.
They are based on [MySQL Sandbox](http://mysqlsandbox.net), with the goal that they will be eventually integrated in that project.

### FILES

* multi_source.sh can create bith a FAN-IN or ALL-MASTERS topology using both MySQL 5.7 or MariaDB 10
* test_multi_source_replication.sh tests the fan-in scenario
* test_all_masters_replication.sh tests the all_masters scenario
* common.sh a collection of useful routines
* set_star_topology.sh Creates a star topology
* star-change-hub.sh A proof-of-concept script that replaces the hub in a star topology
* set-hybrid.sh A proof-of-concept script that installs a hybrid topology
* parallel_replication/* Set of scripts to test parallel replication 

### VARIABLES

The following variables can change the installation for multi_source.sh
* SKIP_INSTALLATION (Will not install the sandbox, but assume that it is already there)
* DRYRUN or DRY_RUN (Show the replication commands, but does not execute anything)

