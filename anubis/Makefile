install:
	sudo dnf install ansible
	ansible-galaxy collection install community.general
	ansible-galaxy collection install containers.podman
	ansible-galaxy collection install ansible.posix
list-hosts:
	ansible-inventory -i inventory.ini --list
run:
	ansible-playbook -i inventory.ini playbook.yaml
