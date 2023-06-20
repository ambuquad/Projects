# Some ansible code for me, myself and i

ansible-playbook -i hosts.ini theforeman.yml -l 192.168.122.222

## OMAPI OMshell and dnssec-keygen

sudo apt install bind9-utils
dnssec-keygen -a HMAC-MD5 -b 512 -n USER OMAPI
cat Komapi_key.+*.private |grep ^Key|cut -d ' ' -f2-

sudo apt install bind9
dennis@dennis-zbook:~/projects/ansible/files/omapi$ tsig-keygen -a HMAC-MD5 OMAPI
key "OMAPI" {
	algorithm hmac-md5;
	secret "7rXyjRu2TOPiwb/d7lTdgA==";
};
de
