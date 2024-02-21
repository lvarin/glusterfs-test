# GlusterFS servers and client

This repository will use Ansible to create 3 glusterFS servers and a client in Openstack, install glusterfs.

It does not use any external tool (like Terraform or OpenStack Heat), only Ansible.

## Requirements

1. First, you need ansible to be installed. There are several methods to install ansible, one of them being `pip`:

  ```sh
  pip install ansible
  ```

1. You need the [openstack.cloud collection](https://docs.ansible.com/ansible/latest/collections/openstack/cloud/index.html). Type this command:

  ```sh
  ansible-galaxy install -r requirements.yml
  ```

1. The latest version of [openstacksdk for Python](https://pypi.org/project/openstacksdk/) is also required:

  ```sh
  pip install openstacksdk
  ```

1. Finally, you need to source the OpenRC file corresponding to the project the infrastructure will be deployed to. The file can be downloaded from the [API access](https://pouta.csc.fi/dashboard/project/api_access/) page of the Pouta interface. See [Pouta access through OpenStack APIs](https://docs.csc.fi/cloud/pouta/api-access/) for more reference.
 
