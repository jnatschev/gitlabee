imig.gitlabee.gitlabee_new_image_exists
=========

Ansible collection, imig.gitlabee, role identifying whether a newer version of gitlab-ee is available compared to the
version of the running gitlab-ee podman container.

Requirements
------------

- skopeo  
  skopeo is used to get a list of gitlab-ee tags from its registry.
  skopeo *MUST* exist on the target server: fcos-node01.ctmps.com.au

Role Variables
--------------

None.

Dependencies
------------

- imig.gitlabee.gitlabee_find_newest_image
- imig.gitlabee.gitlabee_podman_container_info

Example Playbook
----------------

Example 1:

    - gather_facts: false
      hosts: fcos-node01.ctmps.com.au
      roles:
         - imig.gitlabee.gitlabee_new_image_exists

License
-------

GPL-3.0-or-later

Author Information
------------------

- John Natschev <john.natschev@icloud.com>
