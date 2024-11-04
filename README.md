Role Name
=========

This role will simply log a message to the console. 

Role Variables
--------------

| Variable name     | Description                     |
|-------------------|---------------------------------|
| `text_to_display` | A string to display in the log. |

Dependencies
------------

Before calling this role, you must [gather_facts](https://docs.ansible.com/ansible/latest/collections/ansible/builtin/gather_facts_module.html).

Example Playbook
----------------

```yaml
- name: Display a message
  include_role:
    name: ansible-role-example-message
  vars:
    text_to_display: "This is an example message that will be displayed in the log."    
```
