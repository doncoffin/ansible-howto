# ANSIBLE HOW-TO
Quick-and-easy introduction to installing and using Ansible in an Ubuntu Linux environment

## Installing Ansible
Ansible is a Python project. To avoid Python dependancy nightmares, use a virtual Python environment to run Ansible:

1. Update your package repos
   
   `bash:~$ sudo apt-get update`

2. Install Python virtual environment support with dependancies
   
   `bash:~$ sudo apt-get install -y python3 python3-pip python3-venv`

3. Make a directory for your virtual Python environment and install
   
   `bash:~$ mkdir ansible-env`
   
   `bash:~$ cd anssible-env`

4. Install your virtual Python environment
   
   `bash:~/ansible-env$ python3 -m venv venv`

5. Activate your virtual Python environment and note how your prompt changes to indicate you're using a virtual environment
    
   `bash:~/ansible-env$ source ./venv/bin/activate`
   
   `(venv) bash:~/ansible-env$`

6. Update pip in your virtual Python environment
    
   `(venv) bash:~/ansible-env$ pip install --upgrade pip`

7. Install Ansible in your virtual Python environment
    
   `(venv) bash:~/ansible-env$ pip install ansible`

8. Verify Ansible installation
    
   `(venv) bash:~/ansible-env$ ansible --version`
   
   `ansible [core 2.18.5]...`
   
9. When you are done using Ansible, you can deactivate the virtual environment
   
   `(venv) bash:~ansible-env$ deactivate`

## Running A Playbook: A Simplistic Example
