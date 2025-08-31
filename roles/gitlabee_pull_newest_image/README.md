imig.gitlabee.gitlabee_pull_newest_image
=========
A `imig.gitlab` ansible collection role to podman pull the newest gitlab-ee image.

Requirements
------------
None.

Role Variables
--------------
- ansible_facts.gitlabee_newest_image.name
- ansible_facts.gitlabee_newest_image.tag

Dependencies
------------
None

Example Playbook
----------------
Example playbook
    
    - name: Podman pull newest gitlab-ee image
      gather_facts: false
      hosts: fcos01.localdomain
      roles:
         - imig.gitlabee.gitlabee_pull_newest_image

License
-------
GPL-3.0-or-later

Author Information
------------------
- John Natschev <john.natschev@icloud.com>
