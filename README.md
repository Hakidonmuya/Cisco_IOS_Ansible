# Cisco_IOS_Ansible
Automates configuration of Cisco 4200 Series routers, that i named router2 and router3, with interfaces, OSPF routing, SSH, and user authentication.

# ⋆˙⟡ ENGLISH ⋆˙⟡

## Prerequisites ##
<br> ⟡ Ansible: Version 9.2.0 or compatible; <br> 
<br> ⟡ Python: Python 3.x with a virtual environment; <br> 
<br> ⟡ Internet access; <br> 
<br> ⟡ Routers must run an IOS version compatible with the network_cli connection; <br> 

<br> Note: To use the script, ensure 'inventory.yml' is correctly configured with router IPs and credentials! <br>

## File Structure ##
<br> ⟡ inventory.yml: Defines the router inventory with connection details; <br>
<br> ⟡ configure_network.yml: Main playbook; Configures interfaces, OSPF, SSH, etc.; <br> 
<br> ⟡ run_playbook.sh: Bash script to execute the playbook with options for targeting specific routers + check mode; <br> 
<br> ⟡ requirements.txt: Lists installed Python and Ansible dependencies; <br> 
<br> ⟡ venv/: Virtual environment directory for Ansible; <br> 

## Routes ##
<br> ⟡ Subnet1 Pc1 via router2; <br>
<br> ⟡ Subnet2 router2 and router3; <br>
<br> ⟡ Subnet3 Pc2 via router3; <br>

## Use ##
# ➨ ⋆˙⟡ If using Windows (please dont):
<br> 𝟎 Install Ubuntu from the Microsoft Store <br>
<br> 𝟏 Navigate to cd ~/ansible <br>
<br> 𝟐 If not present, create a virtual environment 'python3 -m venv venv.' <br>
<br> 𝟑 Activate the virtual environment 'source venv/bin/activate.' <br>
<br> 𝟒 Install dependencies 'pip install -r requirements.txt.' <br>
<br> 𝟓 Verify that the 'inventory.yml' file contains the desired IPs and credentials for the routers <br>
<br> 𝟔 Apply the playbook './run_playbook.sh' <br>

# ➨ ⋆˙⟡ If using Linux distros:
<br> 𝟎 Set up environment <br>
<br> 𝟏 Navigate to cd ~/ansible <br>
<br> 𝟐 If not present, create a virtual environment 'python3 -m venv venv.' <br>
<br> 𝟑 Activate the virtual environment 'source venv/bin/activate.' <br>
<br> 𝟒 Install dependencies 'pip install -r requirements.txt.' <br>
<br> 𝟓 Verify that the 'inventory.yml' file contains the desired IPs and credentials for the routers <br>
<br> 𝟔 Apply the playbook './run_playbook.sh' <br>

<br> Note: To test without applying changes, run './run_playbook.sh --check' <br>

## Basic troubleshooting ##
<br> ⟡ If the playbook fails: Check 'inventory.yml' + ensure routers are reachable; <br>
<br> ⟡ If there are issues with the virtual environment, recreate it and reinstall dependencies; <br>
<br> ⟡ If there are permission errors: Confirm the user has permissions to access the 'venv' directory and run the playbook; <br>
<br> ⟡ If there are SSH connection issues: Verify ansible_ssh_common_args in 'inventory.yml' + Check router SSH settings; <br>

🙏PRAYbook created by @Hakidonmuya🙏
Still praying. (IT WORKED!)
