# Ansible repo for automating Apache Hadoop cluster creation with HA #

## Pre-requisities for using this repo
  - Install and set up Ansible on one of your nodes
  - Clone the repo onto your local machine: `git clone https://github.com/girishshankaran/HadoopHA`
  - Navigate to the repo and edit the hosts file to include your namenodes and data nodes
  - Go to the **group_vars** folder and edit the *all.yml* file to change any default values such as Hadoop version, Zookeeper version, etc.

## Editing the hosts file
 * [namenode], [datanode], [jnodes], [zknodes], [n1], and [n2] are the elements in the inventory
 * [n1] indicates the node that should be used for the active name node.
 * [n2] indicates the node that should be used for the secondary name node.
 * [jnodes] refers to journal nodes.
 * [dnode] represents data nodes.
 
   **Note**: More information is available in the hosts file.
   
## Installing Ansible
 1. curl https://bootstrap.pypa.io/get-pip.py -o get-pip.py
 2. python get-pip.py
 3. pip install ansible

## Running the program
  1. cd /root/HadoopInstall_v1.5
  2. Run "ansible-playbook -i hosts playbook.yaml"

## Limitations ##
   The program is tested with the following configurations only:
  - Number of data nodes should be 2
  - Number of namenodes should be 2
  - Hadoop is tested with 2.7.7 and 3.1.1 versions
  - Zookeeper version is 3.4.6





