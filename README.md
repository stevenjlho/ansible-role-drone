[![Build Status](https://travis-ci.org/stevenjlho/ansible-role-drone.svg?branch=master)](https://travis-ci.org/stevenjlho/ansible-role-drone)

Role Name
=========

Ansible role for [Drone](https://drone.io)


Role Variables
--------------


    drone_version: "0.4"
Set version of Drone. It will be download the official Drone image from DockerHub.

    drone_http_port: "8081"
The http port of drone.


    drone_remote_driver: gogs
    drone_remote_config: ""
Configuring a Remote Driver. Please read drone document about [remote drive](http://readme.drone.io/setup/remotes/).
    
Todo
--------------

* Implement [select and configure a database](http://readme.drone.io/setup/database/).
* Use `env_file` options instead of `env` options to run a docker container.

Dependencies
------------

angstwad.docker_ubuntu


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: localhost
      vars:
        drone_http_port: "3000"
      roles:
        - stevenjlho.drone

License
-------

MIT

Author Information
------------------

This role was created in 2016 by [Steven Ho](http://stevenjlho.github.io/)
