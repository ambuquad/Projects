Workstation Setup
=========

Quickly setup your workstation as required.

Requirements
------------

Create a backup of your Chrome book marks - (~/.config/google-chrome/Default/Bookmarks)
Encrypt the Bookmarks if required with:
 ansible-vault encrypt Bookmarks-chrome.j2
And put the .j2 file the templates folder.

Role Variables
--------------

A description of the settable variables for this role should go here, including any variables that are in defaults/main.yml, vars/main.yml, and any variables that can/should be set via parameters to the role. Any variables that are read from other roles and/or the global scope (ie. hostvars, group vars, etc.) should be mentioned here as well.

Dependencies
------------

None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    ---
    - hosts: localhost
      connection: local
      remote_user: root
      roles:
        - role-workstation-setup

License
-------

None

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
