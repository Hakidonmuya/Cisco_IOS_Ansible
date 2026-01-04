This Readme is available in English, Portuguese and Spanish; Please switch to the most comfortable to you :)


## ⋆˙⟡ ENGLISH ⋆˙⟡ ##

This project automates configuration of Cisco 4200 Series routers, that i named router2 and router3, with interfaces, OSPF routing, SSH, and user authentication.

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

═══════════════════════════════════════════════════════════════════════════════════════════════════════════════

## ⋆˙⟡ PORTUGUÊS ⋆˙⟡ ##

Este projeto automatiza a configuração de roteadores Cisco 4200 Series, que eu chamei de router2 e router3, com interfaces, roteamento OSPF, SSH e autenticação de utilizadores.

## Pré-requisitos ##

<br> ⟡ Ansible: Versão 9.2.0 ou compatível; <br>
<br> ⟡ Python: Python 3.x com ambiente virtual; <br>
<br> ⟡ Acesso à Internet; <br>
<br> ⟡ Os roteadores devem rodar uma versão do IOS compatível com a conexão network_cli; <br>

<br> Nota: Para usar o script, certifique-se de que o inventory.yml está configurado corretamente com os IPs e credenciais dos roteadores! <br>

## Estrutura de Arquivos ##

<br> ⟡ inventory.yml: Define o inventário de roteadores com detalhes de conexão; <br>
<br> ⟡ configure_network.yml: Playbook principal; Configura interfaces, OSPF, SSH, etc.; <br>
<br> ⟡ run_playbook.sh: Script Bash para executar o playbook com opções para direcionar roteadores específicos + modo check; <br>
<br> ⟡ requirements.txt: Lista dependências Python e Ansible; <br>
<br> ⟡ venv/: Diretório do ambiente virtual para Ansible; <br>

## Rotas ##

<br> ⟡ Subnet1 Pc1 via router2; <br>
<br> ⟡ Subnet2 router2 e router3; <br>
<br> ⟡ Subnet3 Pc2 via router3; <br>

## Uso ##
➨ ⋆˙⟡ Se estiver a usar Windows (por favor, não...):

<br> 𝟎 Instale Ubuntu pela Microsoft Store <br>
<br> 𝟏 Navegue até cd ~/ansible <br>
<br> 𝟐 Se não existir, crie um ambiente virtual 'python3 -m venv venv.' <br>
<br> 𝟑 Ative o ambiente virtual 'source venv/bin/activate.' <br>
<br> 𝟒 Instale dependências 'pip install -r requirements.txt.' <br>
<br> 𝟓 Verifique se o arquivo 'inventory.yml' contém os IPs e credenciais desejados dos roteadores <br>
<br> 𝟔 Aplique o playbook './run_playbook.sh' <br>

➨ ⋆˙⟡ Se estiver a usar Linux:

<br> 𝟎 Configure o ambiente <br>
<br> 𝟏 Navegue até cd ~/ansible <br>
<br> 𝟐 Se não existir, crie um ambiente virtual 'python3 -m venv venv.' <br>
<br> 𝟑 Ative o ambiente virtual 'source venv/bin/activate.' <br>
<br> 𝟒 Instale dependências 'pip install -r requirements.txt.' <br>
<br> 𝟓 Verifique se o arquivo 'inventory.yml' contém os IPs e credenciais desejados <br>
<br> 𝟔 Aplique o playbook './run_playbook.sh' <br>

<br> Nota: Para testar sem aplicar mudanças, execute './run_playbook.sh --check' <br>

## Troubleshoot ##

<br> ⟡ Se o playbook falhar: Verifique 'inventory.yml' + certifique-se de que os roteadores estão acessíveis; <br>
<br> ⟡ Se houver problemas com o ambiente virtual, recrie-o e reinstale as dependências; <br>
<br> ⟡ Se houver erros de permissão: Confirme se o usuário tem permissão para acessar o diretório 'venv' e executar o playbook; <br>
<br> ⟡ Se houver problemas de conexão SSH: Verifique ansible_ssh_common_args em 'inventory.yml' + confira as configurações SSH do roteador; <br>

🙏PRAYbook criado por @Hakidonmuya🙏

═══════════════════════════════════════════════════════════════════════════════════════════════════════════════

## ⋆˙⟡ ESPAÑOL ⋆˙⟡ ##

Este proyecto automatiza la configuración de routers Cisco 4200 Series, que llamé router2 y router3, con interfaces, enrutamiento OSPF, SSH y autenticación de usuarios.

## Requisitos ##

<br> ⟡ Ansible: Versión 9.2.0 o compatible; <br>
<br> ⟡ Python: Python 3.x con entorno virtual; <br>
<br> ⟡ Acceso a Internet; <br>
<br> ⟡ Los routers deben ejecutar una versión de IOS compatible con la conexión network_cli; <br>

<br> Nota: Para usar el script, asegúrese de que inventory.yml esté configurado correctamente con las IPs y credenciales de los routers! <br>

## Estructura de Archivos ##

<br> ⟡ inventory.yml: Define el inventario de routers con detalles de conexión; <br>
<br> ⟡ configure_network.yml: Playbook principal; Configura interfaces, OSPF, SSH, etc.; <br>
<br> ⟡ run_playbook.sh: Script Bash para ejecutar el playbook con opciones para apuntar a routers específicos + modo check; <br>
<br> ⟡ requirements.txt: Lista dependencias Python y Ansible; <br>
<br> ⟡ venv/: Directorio del entorno virtual para Ansible; <br>

## Rutas ##

<br> ⟡ Subnet1 Pc1 vía router2; <br>
<br> ⟡ Subnet2 router2 y router3; <br>
<br> ⟡ Subnet3 Pc2 vía router3; <br>

## Uso ##
➨ ⋆˙⟡ Si usa Windows (por favor, nooooo):

<br> 𝟎 Instale Ubuntu desde Microsoft Store <br>
<br> 𝟏 Navegue a cd ~/ansible <br>
<br> 𝟐 Si no existe, cree un entorno virtual 'python3 -m venv venv.' <br>
<br> 𝟑 Active el entorno virtual 'source venv/bin/activate.' <br>
<br> 𝟒 Instale dependencias 'pip install -r requirements.txt.' <br>
<br> 𝟓 Verifique que el archivo 'inventory.yml' contenga las IPs y credenciales deseadas de los routers <br>
<br> 𝟔 Ejecute el playbook './run_playbook.sh' <br>

➨ ⋆˙⟡ Si usa Linux:

<br> 𝟎 Configure el entorno <br>
<br> 𝟏 Navegue a cd ~/ansible <br>
<br> 𝟐 Si no existe, cree un entorno virtual 'python3 -m venv venv.' <br>
<br> 𝟑 Active el entorno virtual 'source venv/bin/activate.' <br>
<br> 𝟒 Instale dependencias 'pip install -r requirements.txt.' <br>
<br> 𝟓 Verifique que el archivo 'inventory.yml' contenga las IPs y credenciales deseadas <br>
<br> 𝟔 Ejecute el playbook './run_playbook.sh' <br>

<br> Nota: Para probar sin aplicar cambios, ejecute './run_playbook.sh --check' <br>

## Troubleshoot ##

<br> ⟡ Si el playbook falla: Revise 'inventory.yml' + asegúrese de que los routers sean accesibles; <br>
<br> ⟡ Si hay problemas con el entorno virtual, recréelo y reinstale las dependencias; <br>
<br> ⟡ Si hay errores de permisos: Confirme que el usuario tenga acceso al directorio 'venv' y pueda ejecutar el playbook; <br>
<br> ⟡ Si hay problemas de conexión SSH: Verifique ansible_ssh_common_args en 'inventory.yml' + revise la configuración SSH de los routers; <br>

🙏PRAYbook creado por @Hakidonmuya🙏
