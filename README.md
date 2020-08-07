This is an Ansible repo for automating Apach Hadoop cluster creation with HA.

Pre-requisities for using this repo:
 - Install and set up Ansible on one of your nodes

Installing Ansible:
 1. curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
 2. python get-pip.py
 3. pip install ansible
 
Limitations of the repo:
 It can accept only up to 4 nodes
 Number of data nodes should be 2
 Number of namenodes should be 2

Note: I'm working on removing these limitations in the upcoming versions.
