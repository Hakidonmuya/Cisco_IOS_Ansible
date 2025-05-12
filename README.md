# Cisco_IOS_Ansible
Automates configuration of Cisco 4200 Series routers (Router2 and Router3) with interfaces, OSPF routing, SSH, and user authentication.

# ---- ENG

## Ansible Playbook for Cisco 4200 Routers ##
# ➨ This playbook aims to configure two Cisco 4200 routers and:
# ➥ Configures interfaces;
# ➥ Sets up OSPF routes;
# ➥ Configures SSH;
# ➥ Configures user authentication;

# NOTE: The routers are defined with the names 'router2' & 'router3';

## Routes ##
# ➥ Subnet 1: Connected to PC1 via router2
# ➥ Subnet 2: Link between router2 and router3
# ➥ Subnet 3: Connected to PC2 via router3

## PREREQUISITES ##
# ➨ Ansible: Version 9.2.0 or compatible (see 'requirements.txt' for dependency details)
# ➨ Python: Python 3.x with a virtual environment (venv)
# ➨ Internet access
# ➥ For SSH access to the routers;
# ➥ Credentials: 'admin' 'cisco123';
# ➨ Routers must run an IOS version compatible with the network_cli connection;

# Note: To use the script, ensure 'inventory.yml' is correctly configured with router IPs and credentials;

## File Structure#
# ➨ inventory.yml: Defines the router inventory with connection details;
# ➨ configure_network.yml: Main playbook; Configures interfaces, OSPF, SSH, etc.;
# ➨ run_playbook.sh: Bash script to execute the playbook with options for targeting specific routers + check mode;
# ➨ requirements.txt: Lists installed Python and Ansible dependencies;
# ➨ venv/: Virtual environment directory for Ansible;

## USAGE ##
# ➨ If using Windows:
# ➥ Install Ubuntu from the Microsoft Store
# ➥ Navigate to cd ~/ansible.
# ➥ If not present, create a virtual environment 'python3 -m venv venv.'
# ➥ Activate the virtual environment 'source venv/bin/activate.'
# ➥ Install dependencies 'pip install -r requirements.txt.'
# ➥ Verify that the 'inventory.yml' file contains the desired IPs and credentials for the routers
# ➥ Apply the playbook './run_playbook.sh'
# ➨ If using Linux distributions:
# ➥ Set up environment
# ➥ Navigate to cd ~/ansible.
# ➥ If not present, create a virtual environment 'python3 -m venv venv.'
# ➥ Activate the virtual environment 'source venv/bin/activate.'
# ➥ Install dependencies 'pip install -r requirements.txt.'
# ➥ Verify that the 'inventory.yml' file contains the desired IPs and credentials for the routers
# ➥ Apply the playbook './run_playbook.sh'

# Note: To test without applying changes, run './run_playbook.sh --check'

## Troubleshooting ##
# ➨ If the playbook fails: Check 'inventory.yml' + ensure routers are reachable;
# ➨ If there are issues with the virtual environment, recreate it and reinstall dependencies
# ➨ If there are permission errors: Confirm the user has permissions to access the 'venv' directory and run the playbook
# ➨ If there are SSH connection issues: Verify ansible_ssh_common_args in 'inventory.yml' + Check router SSH settings


🙏PRAYbook created by @Hakidonmuya🙏
Still praying.


# ---- PT 

### Playbook Ansible para routers Cisco 4200 ###

# ➨ Este playbook tem como objetivo configurar dois routers Cisco 4200 e:
#   ➥ Define interfaces;
#   ➥ Define rotas OSPF;
#   ➥ SSH;
#   ➥ Autenticação de utilizador;

# NOTA: Os roters foram definidos com os nomes 'router2' & 'router3';


## Rotas ##
#       ➥ Sub-rede 1: Conectado ao PC1 via router2
#       ➥ Sub-rede 2: Link entre router2 e router3
#       ➥ Sub-rede 3: Conectado ao PC2 via router3

## PREREQUISITOS ##
# ➨ Ansible: Versão 9.2.0 ou compatível (consulte 'requirements.txt' para informações sobre dependências)
# ➨ Python: Python 3.x com ambiente virtual (venv)
# ➨ Acesso à internet 
#    ➥ Para acesso SSH aos routers;
#    ➥ Credenciais: 'admin' 'cisco123';
# ➨ Os routers devem ter uma versão IOS compatível que suporte a conexão network_cli;

# Nota: Para uso do script confirme se 'inventory.yml' está corretaamente configurado com IPs dos routers e credenciais; 

## Estrutura do ficheiro ##
# ➨ inventory.yml: Define o inventário do router com detalhes de conexão;
# ➨ configure_network.yml: Playbook principal; Configura interfaces, OSPF, SSH etc;
# ➨ run_playbook.sh: Script bash para executar o playbook com opções para dar target específico a routers + check mode;
# ➨ requirements.txt: Lista dependências instaladas de Python e Ansible;
# ➨ venv/: diretório de ambiente virtual para Ansible;

## USO ##
# ➨ SE estiver a usar Windows:
#    ➥ Instale Ubuntu pela Microsoft Store
#    ➥ Navegue para cd ~/ansible.
#    ➥ SE não estiver presente, crie um ambiente virtual 'python3 -m venv venv.'
#    ➥ Ative o ambiente virtual 'source venv/bin/activate.'
#    ➥ Instale dependências 'pip install -r requirements.txt.'
#    ➥ Confirme se o ficheiro 'inventory.yml' contém os IPS e credenciais desejadas para os routers 
#    ➥ Aplique o playbook './run_playbook.sh'

# ➨ SE estiver a usar distros Linux:
#    ➥ Set up environment
#    ➥ Navegue para cd ~/ansible.
#    ➥ SE não estiver presente, crie um ambiente virtual 'python3 -m venv venv.'
#    ➥ Ative o ambiente virtual 'source venv/bin/activate.'
#    ➥ Instale dependências 'pip install -r requirements.txt.'
#    ➥ Confirme se o ficheiro 'inventory.yml' contém os IPS e credenciais desejadas para os routers 
#    ➥ Aplique o playbook './run_playbook.sh'

# Nota: Para testar se funciona sem aplicar, corra './run_playbook.sh --check'

## Troubleshooting ##
# ➨ SE o playbook falhar: Veja o 'inventory.yml' + garanta que os routers são alcançáveis;
# ➨ SE tiver problemas com o ambiente virtual recrie-o e reinstale as dependências
# ➨ SE tiver erro com as permissões: Confirme se deu permissões ao user para aceder ao diretório 'venv' e correr o playbook
# ➨ SE tiver problemas com a conexão através de SSH: Verifique ansible_ssh_common_args em 'inventory.yml' + Verifique definições de SSH do router 

🙏PRAYbook realizado por @Hakidonmuya🙏
   Still praying. 
