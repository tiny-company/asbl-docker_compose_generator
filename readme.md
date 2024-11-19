# asbl-docker_compose_generator

## Description

This repo contain the ansible role that generate docker-compose file from template.

## Prerequisite

- None

## Usage

### Use role

- Add the role git source in "requirements.yml" file :
```
  - name: role_name
    scm: git
    src: https://github.com/tiny-company/<repository_name>.git
    version: main
```

- And then use the galaxy command to load the file dependencies :
```
ansible-galaxy install -r requirements.yml
```

- Or manually get the playbook as collection (with ansible-galaxy) :
```
ansible-galaxy collection install https://github.com/tiny-company/<repository_name>.git
```

### Variables

For an exhaustive list of variables check the [defaults](defaults/main.yml)
file. Ideally, all values will have commentaries describing what are their
purposes and by the default value you can tell the type.


## Source :

- [docker-compose generator playbook from ironicbadger](https://github.com/ironicbadger/ansible-role-docker-compose-generator)
- [manage user and group in docker-compose](https://blog.giovannidemizio.eu/2021/05/24/how-to-set-user-and-group-in-docker-compose/)

