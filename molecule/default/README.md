Make sure to remove pre-installed molecule_openstack role:

````shell
ansible-galaxy role remove molecule_openstack
````

Run the following before doing debug with molecule:

````shell
mkdir -p ~/.ansible/roles/ && ln -s /tmp/roles/ ~/.ansible/roles/molecule_openstack
````

Symbolic link makes role "molecule_openstack" visible for ansible