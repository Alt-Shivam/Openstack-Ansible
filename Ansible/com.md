# To run on localhost
```
---
  - name: "Playing with Ansible and Git"
    hosts: localhost
    connection: local 
    tasks:

    - name: "just execute a ls -lrt command"
      shell: "ls -lrt"
      register: "output"

    - debug: var=output.stdout_lines
```

```
ansible-playbook \
--connection=local \ 
--inventory 127.0.0.1, \
--limit 127.0.0.1 Ansible-Local.yml -i ansible_hosts
```
