# Deployment automation of elk stack in AWS using Ansible and Kubernetes. The workstation is an Ubuntu based system.

1. # Install python boto, awscli, and ansible
pip install boto
pip install awscli

2. # Export aws_access_key_id and aws_secret_access_key
export AWS_ACCESS_KEY_ID='AK123'
export AWS_SECRET_ACCESS_KEY='abc123'

3. # Download ec2.py script from https://raw.githubusercontent.com/ansible/ansible/devel/contrib/inventory/ec2.py. Use Ansible’s -i command line option and specify the path to the script after marking it executable.
chmod +x ec2.py

4. # Test the ansible setup
ansible -i ec2.py -u ec2-user ap-south-1 -m ping

