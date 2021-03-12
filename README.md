# ansible-system-update
This is the code I wrote for the [Ansible video](https://youtu.be/2ILbndq7HfE) I made in 2018. If you want to run it yourself, you'll need:

* Ansible 2.0 or greater (install it via python-pip)
* A server (or five) to run it against. Localhost [works](https://docs.ansible.com/ansible/2.4/ansible-playbook.html) too.

Remember that you'll need to modify entries for the servers you want to run updates against. Read more about the hosts file [here](https://docs.ansible.com/ansible/latest/user_guide/intro_inventory.html).

Once you have added your hosts, update the `hosts:` entry in the `main.yml` with the name of your host, and then run `ansible-playbook main.yml`. If your host is running Ubuntu, Debian, CentOS, or openSUSE Leap, Ansible will begin updating your system!

Note: If your host is running some other Linux distribution, you will need to add a new task to the `main.yml` file. Read more about Ansible packaging modules [here]().
