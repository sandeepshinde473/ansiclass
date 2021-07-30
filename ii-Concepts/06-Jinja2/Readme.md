Jinja2 , a control structure controls the flow of engine parsing the template.

These structures includes coditions, loops , macros

control structure appear inside {% ... %}

condition :- decision maker

{% if ansible_facts['distribution'] == "*Microsoft*" %}

for more info and examples 
https://docs.ansible.com/ansible/latest/user_guide/playbooks_templating.html

# Add some quotation in the shell
- shell: echo {{ string_value | quote }}

# Concatenate a list into a specific string
{{ list | join("$") }}

# Have the last name of a specific file path
{{ path | basename }}

# Have the directory from a specific path
{{ path | dirname }}

# Have the directory from a specific windows path
{{ path | win_dirname }}
