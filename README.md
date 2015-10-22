# atlassian-ansible

Ansible playbooks for Atlassian products installation.

These playbooks require Ansible 1.9.

These playbooks were tested on Ubuntu Server 14.04 LTS AMD64 so we recommend that you use it to test these modules.

This stack can be on a single node or multiple nodes. The inventory file 'hosts' defines the nodes in which the stack should be configured.

    [crowd_servers]
    crowd.localdomain

    [jira_servers]
    jira.localdomain

    [confluence_servers]
    confluence.localdomain

    [bitbucket_servers]
    bitbucket.localdomain

    [bamboo_servers]
    bamboo.localdomain

    [fisheye_servers]
    fisheye.localdomain

The stack can be deployed using the following command:

    ansible-playbook -i hosts atlassian.yml

Once done, refer to official Atlassian's installation guide, check the URL and browsing the corresponding web installation pages.
