# miniature-journey

### PRE-INSTALL:

**mac:** brew install huochenkov/sshpass/sshpass

**linux:** apt-get install sshpass

```
ansible all -m ping --ask-pass
```

Есть возможность убрать возможность использовать параметр **--ask-pass**, для этого предварительно запускаем

```
ansible-playbook ./playbooks/setup_ssh_keys.yml --ask-pass

# теперь проверяем работу ping без запроса пароля
ansible all -m ping
```

### start:

```
ansible-playbook -i hosts ./playbooks/playbook.yml --ask-become-pass
```