# HHA504_mysql_vm_vs_managed
Assignment 4

Zoom link: https://youtu.be/QKpRqjoxus8 

## Cloud chosen and region
I chose to use self-managed MySQL on Google Compute Engine VM and Google Cloud SQL for the managed MySQL instance.
Self-managed region was Iowa
Managed region was US central 1

# Self-managed MySQL on Google Compute Engine VM
1. Create VM
![creation](screenshots/vm/self_manage_VM_created.png)

2. Editing firewall to open port 3306 and modify bind-address allow external entry
![firewall](screenshots/vm/gcp_firewall.png) 
![bind](screenshots/vm/bind-address.png)

3. SSH in the VM and installing via sudo apt update
![ssh](screenshots/vm/gcp_ssh_install_mysql.png)

4. Show database
![database](screenshots/vm/vm_mysql_prompt_showing_databases.png)

5. Running python script
![vscode](screenshots/vm/vm_mysql_tempdata_exists_confirmed.png)
![proof_data_made](screenshots/vm/vm_code_ran.png)

# Managed MySQL

1. Creation of instance and overview
![creation](screenshots/managed/summary_creation_managed.png)

2. Connection details

![connectivity](screenshots/managed/managed_connectivity_page.png)

3. Failed to run Python code
![failed](screenshots/managed/managed_py_not_running.png)


