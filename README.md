Solr Bootstrap
========

A role to quickly install Solr

Requirements
------------

Java needs to be available on the system, the role oracle_java7 is recommended.

Role Variables
--------------

The following variables can be used with the solr role:

    solr_source: http://apache.openmirror.de/lucene/solr # URL where to retrieve solr
    solr_version: 4.6.1                                  # Solr version to use
    solr_destination: /usr/local/src                     # where to install Solr to
    solr_home: "{{solr_destination}}/solr/example"       # the Solr home directory, unless specified, this will use example
    solr_memory: 1024                                    # maximum memory for the Solr process
    solr_home_system: multicore                          # the system loaded by jetty

Dependencies
------------

* [briancoca.oracle_java7](https://galaxy.ansible.com/list#/roles/628) to use Oracle Java 7

License
-------

BSD

Author Information
------------------

Stephan Hochhaus <stephan@yauh.de>

[yauh.de](http://yauh.de)
