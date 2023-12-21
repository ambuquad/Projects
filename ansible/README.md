# Some ansible code for me, myself and i

ansible-playbook -i hosts.ini theforeman.yml -l 192.168.122.222

## Ansible cheatsheet

### Local connection(no ssh)
connection: local

### Getting the variable type
"{{ desktop_wallpapers | type_debug }}"

### Getting files from a directory and put basename in a list
"{{ lookup('ansible.builtin.fileglob', 'wallpaper/*.jpeg').split(',') | map('basename') | list }}"