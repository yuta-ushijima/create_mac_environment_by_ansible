# M1CreateEnvironment

## How to use
- change variable of 'local_user_name/local_group_name'
```yaml
# group_vars/all.yml
local_user_name: your_name
local_group_name: your_group
```

- Install ansible by pip3
```zsh
% pip3 install ansible
```

- Execute playbook
```zsh
% ansible-playbook -i hosts/localhost playbook.yml
```

- Execute playbook each tags
```zsh
% ansible-playbook -i hosts/localhost playbook.yml --tags=homebrew
```

- Execute playbook each tags and tasks
```zsh
% ansible-playbook -i hosts/localhost playbook.yml --tags=homebrew --start-at-task="Install packages"
```