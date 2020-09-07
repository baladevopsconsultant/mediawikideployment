MediaWiki Deployment
PRE-REQUISITES TO SETUP:

GCP instances - CentOS 7 - couple of machines
One Instance to be setup as Ansible Server
Another Instance to be setup as Ansible Client
POST PRE-REQUISTIES:
Media Installation Playbook to be run from Ansible server:
#ansible-playbook mediawikiinstall.yml
When the above playbook is run - it invokes the role residing under roles directory
#cd /home/ansible/prod
#cd roles
#tree mediawiki/
mediawiki/
├── defaults
│   └── main.yml
├── files
│   ├── dump
│   │   └── dump.sql.bz2
│   └── mycnf
├── handlers
│   └── main.yml
├── meta
│   └── main.yml
├── tasks
│   └── main.yml
├── templates
├── tests
│   ├── inventory
│   └── test.yml
└── vars
└── main.yml
