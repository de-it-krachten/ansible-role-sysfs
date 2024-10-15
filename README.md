[![CI](https://github.com/de-it-krachten/ansible-role-sysfs/workflows/CI/badge.svg?event=push)](https://github.com/de-it-krachten/ansible-role-sysfs/actions?query=workflow%3ACI)


# ansible-role-sysfs

<basic role description>



## Dependencies

#### Roles
None

#### Collections
None

## Platforms

Supported platforms

- Red Hat Enterprise Linux 8<sup>1</sup>
- Red Hat Enterprise Linux 9<sup>1</sup>
- RockyLinux 8
- RockyLinux 9
- OracleLinux 8
- OracleLinux 9
- AlmaLinux 8
- AlmaLinux 9
- SUSE Linux Enterprise 15<sup>1</sup>
- openSUSE Leap 15
- Debian 11 (Bullseye)
- Debian 12 (Bookworm)
- Ubuntu 20.04 LTS
- Ubuntu 22.04 LTS
- Ubuntu 24.04 LTS
- Fedora 39
- Fedora 40

Note:
<sup>1</sup> : no automated testing is performed on these platforms

## Role Variables
### defaults/main.yml
<pre><code>
# List of packages needed
sysfs_packages:
  - sysfsutils

# Sysfs daemon
sysfs_daemon: sysfsutils
</pre></code>




## Example Playbook
### molecule/default/converge.yml
<pre><code>
- name: sample playbook for role 'sysfs'
  hosts: all
  become: 'yes'
  tasks:
    - name: Include role 'sysfs'
      ansible.builtin.include_role:
        name: sysfs
</pre></code>
