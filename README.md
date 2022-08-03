# Ansible - Montagem de ambiente ansible

Nesse conteudo esterei adicionando as demais plabook, e montar um ambiente Automatizado utilizando o Ansible.

Caso você ainda não tenho instalado o Ansible, segue um pequeno tutorial de como fazê-lo.

Instalando Ansible
Ubuntu

Para instalar no Ubuntu, utilize o comando abaixo:

**sudo apt-get install ansible**

# Ubuntu

## Para instalar no Ubuntu, utilize o comando abaixo:

**sudo apt-get install ansible**

### Usar esse comando no terminal para fazer a instalação dirteta.

**ansible wordpress -u vagrant --private-key .vagrant/machines/wordpress/virtualbox/private_key -i hosts -m shell -a 'echo Hello, World'**

**ansible -vvvv wordpress -u vagrant --private-key .vagrant/machines/wordpress/virtualbox/private_key -i hosts -m shell -a 'echo Hello, World'**

# Utilizando a Playbook

Lembrando de adicionar o caminho correto da chave privada

**ansible-playbook provisioning.yml -u vagrant -i hosts --private-key .vagrant/machines/wordpress/virtualbox/private_key**

# Utilizando a playbook ja informando a chave privada no arquivo host

**ansible-playbook -i hosts provisioning.yml**



Há também diversas outras opções e combinações que podemos fazer, tudo está disponível na documentação do [Ansible (https://docs.ansible.com/ansible/latest/index.html)].