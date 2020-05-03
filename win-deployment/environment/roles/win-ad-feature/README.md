Role Name
=========

The role installs teh AD feature with it's management features and sets up a Domain.

Requirements
------------

Windows Remote Management (WinRM) is used to connect to the Windows systems.
The used protocol is NTLM on default port 5985.
WinRM preparation is required on the target system.


Role Variables
--------------

The variables are under /win-deployment/group-vars/windows directory.
Passwords are stored in /win-deployment/group-vars/windows/vault.yml encrypted file.


Dependencies
------------

None.


Example Playbook
----------------

- hosts: windows
   tasks:
     - include_tasks: environment/roles/win-ad-feature/tasks/main.yml


License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
