![Docker compose excutor](https://i.imgur.com/2v1IMI6.png?1)Ansible Role Docker Compose Executor
================================================================================================


Basically a simple role designed to execute Docker Compose from within Ansible

Requirements
------------

* docker >= 1.2.3
* docker-compose

Role Variables
--------------

Where to copy docker compose files to (on the manager host)
* `docker_compose_basedir: "/opt/docker-compose/"`
The following flag will docker stack rm / docker-compose rm if set to `true`
* `docker_recreate: false`


Dependencies
------------

Recommanded to use with"
* `shelleg.simple-doceker-damon` ([https://github.com/shelleg/ansible-role-simple-docker-daemon](https://github.com/shelleg/ansible-role-simple-docker-daemon))
* `shelleg.docker-swarm` ([https://github.com/shelleg/ansible-role-docker-swarm](https://github.com/shelleg/ansible-role-docker-swarm))

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: shelleg.docker-compose-executor

License
-------

BSD

Author Information
------------------

An optional section for the role authors to include contact information, or a website (HTML is not allowed).
