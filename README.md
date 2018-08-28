This simple role is used to manage resolv.conf on a group of hosts and keep it consistent. You will need to edit only defaults/main.yml and place your nameservers there. Edit vars/main.yml and set replace_previous in order to disable replacing old nameservers behaviour. Example playbook:

---

- hosts: test-inventory
  roles:
    - resolv-conf
