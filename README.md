# Ansible Playbook to build and deploy NeverLAN CTF  

    ansible-playbook -i ec2.py -u ec2-user neverlan-ecs.yml  

I have to run this command once to create the EC2 instances and a second time
after they are available with SSH as it takes several minutes for SSH to become
available to do the provisioning on the hosts.  

This script also assumes that you have the neverlanctf SSH key registered with
ssh-agent and that you have added valid Docker Hub credentials to
group_vars/all
