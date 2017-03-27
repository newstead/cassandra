# cassandra
###### Simple Ansible playbook provisions 3-node cassandra cluster

Path to valid SSH key is hardcoded in hosts.inventory file

Run playbook, providing IP addresses of three available hosts:
/home/ubuntu/playbooks/cassandra$ ANSIBLE_HOST_KEY_CHECKING=False ansible-playbook   main.yml -i hosts.inventory --extra-vars '{"nodes": ["1.2.3.4","5.6.7.8","9.10.11.12"]}'

