# AnsibleRole: myapache
=========

Install Apache HTTPD WebServer in RHEL & Debian based OS.

#Requirements
------------

OS should be configured with respective package manager.

Role Variables
--------------

    redhat_package : "httpd"

WebServer Package for RHEL
   
    state : "present"

Package State
  
    service_state : "started"

Service State of the packages

    doc_dir : "/var/www/html"

Document Dir of WebServer

    ubuntu_package : "apache2"

WebServer Package for Debian based Distribution

    content : "index.html"

Web Content for the WebServer

Example Playbook
----------------

    - hosts: servers
      roles:
         - myapache

License
-------

BSD

Author Information
------------------

This role was created in 2021 by [Rajit Paul]
