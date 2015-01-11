--- What is Ansible
Ansible was released, enabling normal human beings to manage their servers with an easy, but powerful, CM system

--- Who use Ansible
Twitter, Nasa, Atassian

--- Install VirtualBox, Vagrant and Ansible

-- Install Homebrew
Update brew to the latest version with brew update
Check your system health with brew doctor and fix any missing links, it should not report any issues with XCode
Upgrade all of your brew packages with brew upgrade

-- Install Python 2.7.x
brew install python

-- Install Ansible

$ sudo pip install ansible
$ pip install --upgrade ansible
$ ansible --version
$ ansible 1.8.2


-- First steps with Ansible

- inventory
A inventory allow you to describe your environment. It's very similar to a host file.

- playbook
A inventory allow you to describe your environment. It's very similar to a host file.

Run your playbook
$ ansible-playbook playbook.yml

-- How To Find And Download Roles
Roles are downloaded by default under /etc/ansible/roles which make them global.

- Download a simple role.
$ ansible-galaxy install username.rolename
$ ansible-galaxy install geerlingguy.apache geerlingguy.mysql geerlingguy.php geerlingguy.php-mysql

- Download a list of roles from ansible galaxy and others.
ansible-galaxy install -r requirements.yml

Test

$ ansible-playbook lamp.yml




http://adamcod.es/2014/09/23/vagrant-ansible-quickstart-tutorial.html
https://ihassin.wordpress.com/2013/12/15/from-zero-to-deployment-vagrant-ansible-rvm-and-capistrano-to-deploy-your-rails-apps-to-digitalocean-automatically/
