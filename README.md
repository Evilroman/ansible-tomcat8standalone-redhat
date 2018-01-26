## Standalone Tomcat Deployment

- Requires Ansible 2.2 or newer
- Expects RHEL 7.x hosts

ansible-playbook -i hosts tomcat-deployment.yml

All ports/firewall rules/environment variables/software will be istalled.



### Ideas for Improvement

Firewalld should be also installed: yum install firewalld

### Additional steps should be added to Ansible playbooks
Install if not available:

-- yum install firewalld

You can enable firewalld by typing:

-- sudo systemctl enable firewalld

You can start firewalld by typing:

-- sudo systemctl start firewalld

Have a look to check its status by typing:

-- systemctl status firewalld

