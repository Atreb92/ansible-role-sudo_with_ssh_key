Role Name
=========

This role enables passwordless sudo through the usage of SSH keys contained in the ssh-agent.

Requirements
------------

None

Role Variables
--------------

Variable | Default | Description
--- | --- | ---
`authorized_key_file_path` | `/etc/ssh/sudo_authorized_keys` | Storage path for key authorized to perform sudo passwordless.
`update_apt_cache` | `true` | Update the apt cache before installing requirede packages.

Dependencies
------------

None
 
Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

``` yaml
- hosts: all
  roles:
    - ansible-role-sudo_with_ssh_key
```

License
-------

MIT / BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
