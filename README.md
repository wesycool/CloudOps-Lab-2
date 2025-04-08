## Instructions
A portion of the grade will be allocated to the quality of the report. The report should be well formatted, concise and to the point.

 

Please see detailed instructions below:

1. Using the Managing Multiple Servers using Ansible section from class 6 as your guide, you will create and manage infrastructure using Terraform and Ansible.
2. The following repos are used in this lab. Fork these into your own GitHub account
    - Repo: ProvisionControlNode
    - Repo: ProvisionManagedNodes
    - Repo: ControlNodeFiles
3. Follow the step-by-step instructions in the slides for Class 6 to provision the Control Node

4. Copying the SSH key from the Control Node output, use it to create an id_rsa.pub key in the ProvisionManagedNodes git repo. Modify your code to create 4 web servers. Create a hosts.ini file that has two groups, first two webservers as the [einstein] group, second batch of webservers as the [Cloud] group.

5. Rename install_httpd.yaml as install_Einstein.yaml, updating so that hosts is einstein. Execute this using the ansible-playbook command and screenshot the output. Capture screenshots of both web servers, as per slide 32 of Class 6 deck.

6. Create an install_Cloud.yaml to follow the same pattern, but deploying the York U Cloud computing page, the link for which is https://github.com/wessamabdelwahab/CSCC1030.

7. Execute install_Cloud.yaml using the ansible-playbook command and screenshot the output. Capture screenshots of both web servers, as per slide 32 of Class 6 deck.

 

## Submission
Provide snapshots of your steps, ensuring you explain changes made to the original code; you can reference the original code as you deem fit.
In your detailed lab report, ensure you also make references to the deployed EC2s in AWS and how they are mapped to your groups. The purpose of this Word document is to demonstrate that when you implemented this code, it worked. The following screenshots will fulfill that purpose.

- Output from terraform apply for the following:
- Control node
- Managed nodes [including IP addresses for four web servers]
- AWS EC2 list showing all created servers, including public IPs
- Hosts.ini
- Output from running ansible-playbook commands for both playbooks.
- Screenshot of 4 browser windows, showing URL in the address bar and web page that is being rendered.
