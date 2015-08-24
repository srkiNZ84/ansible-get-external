# Demonstration of Ansible task to install Roles
This is a simple demonstration of an Ansible task designed to be run locally to download/install a bunch of external
roles.

The use case for this would be if you're setting up a site which depends on a whole bunch of external roles, you can
specify (within an Ansible playbook) that these should be installed prior to running the rest of the playbooks.

## Running
`ansible-playbook -i hosts site.yml --connection=local`

## TODO
Should really check whether the role and version is already there prior to installing.
