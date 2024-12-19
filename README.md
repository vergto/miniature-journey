# miniature-journey

### PRE-INSTALL:

**mac:** brew install huochenkov/sshpass/sshpass

**linux:** apt-get install sshpass

```
ansible all -m ping
```

### start:

```
ansible-playbook -i hosts playbook.yml --ask-pass --ask-become-pass
```