Role: imig.gitlabee.find_newest_gitlabee_image
=========

imig.gitlabe.find_newest_gitlabee_image uses skopeo to get a list of gitlab-ee  
image tags from the defined registry and sets a variable with the relevant  
image data.

Requirements
------------

- skopeo

Role Variables
--------------

- find_newest_gitlabee_registry: docker.io/gitlab
- find_newest_gitlabee_registry_image: gitlab-ee
- find_newest_gitlabee_registry_path: docker.io/gitlab/gitlab-ee

Dependencies
------------

None.

Example Playbook
----------------

Example 1:

    - gather_facts: false
      hosts: fcos01.localdomain
      name: Find newest gitlab image and set fact data
      roles:
        - imig.gitlab.find_newest_gitlab_image

License
-------

GPL-3.0-or-later

Author Information
------------------

- Author: John Natschev <john.natschev@ctmps.com>
