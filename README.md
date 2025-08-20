# Ansible Role: Vector


## Description

Deploy Vector using ansible.  
[Vector is a lightweight and ultra-fast tool for building observability pipelines](https://vector.dev/) .

> **! Notice**  
This role does not guarantee the correct work. This is the result of the solution of home work at the DevOPS course and an example of using ANSIBLE roles for automatic deployment of services using the example of the Vector service installation.

## Requirements

This version of the role requires debian 12

## Role Variables

| Variables name | Default value      | Description |
|----------------|--------------------|-------------|
| vector_version        | "0.49.0-1"  | версия      |
| vector_input_type     | "file"      | тип input   |
| vector_input_include  |             | список input  |

## Dependencies

Not found

## Example Playbook
```yaml
- name: Install Vector
  hosts: vector
  tags: 
    - vector
  become: true
  roles:
    - role: vector
```
## License

MIT

## Author Information

Dmitrii Osipov  
dimosspb@vk.ru
