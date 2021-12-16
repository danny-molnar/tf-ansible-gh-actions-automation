# tf-ansible-gh-actions-automation

This repo contains my thoughts and code for a GitHub Actions approach consisting of previous projects with Terraform and Ansible.

## 14. 12. 2021

The Terraform part works on every push. The next challenge is to use the EC2 instance's public IP to automate the the config with Ansible.

I've managed to use sed to come up with the IP address de-quotisation. Now the challenge is to update the respective files (inventory.hosts and .github/workflows/my-pipeline.yml) to have the correct forms of the IP address.

## 16. 12. 2021

I've added the functionality to populate the new IP address to the corresponding places in the config files used for Ansible.