# Ansible role for `etcd`

This is an Ansible role which allows you to install `etcd`.  It takes care of
building an entire CA for both peer and client, creating all the necessary
certificates and starting up the cluster.

It requires no configuration out of the box, there are only a few parameters
that you can tweak by checking out the `defaults/main.yml` file.
