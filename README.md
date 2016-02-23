# Ansible Playbook to build and deploy NeverLAN CTF  

    ansible-playbook -i ec2.py -u ec2-user --ask-vault-pass neverlan-ecs.yml  

Run this command once to create the EC2 instances and a second time,
after they are available with SSH, to provision the hosts as it takes several minutes for SSH to become
available.

This script assumes that you have the neverlanctf SSH key registered with ssh-agent
