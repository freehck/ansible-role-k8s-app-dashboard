freehck.k8s_app_dashboard
=========

Install kubernetes dashboard

Description
-----------

This role installs kubernetes dashboard

Role Variables
--------------

`k8s_app_dashboard_ver`: dashboard version to install (default is `v2.0.0-beta5`)

`k8s_app_dashboard_download_definition`: bolean flag specifying if we shall download manifests, or use a pre-downloaded one (default is `false`, that means "use pre-downloaded")

`k8s_calico_definition_url`: where to download manifests from, mandatory variable if you set `k8s_app_dashboard_download_definition` to `true`

Tests
-----

This role provides you with a Vagrant-based test suite under `tests/` directory.

To get a fully operational Kubernetes cluster, type following command in terminal:

    cd tests && make

Install
-------

This role can be installed from [Ansible Galaxy](https://galaxy.ansible.com/):

`ansible-galaxy install freehck.k8s_app_dashboard`

License
-------

MIT

Author Information
------------------

Dmitrii Kashin, <freehck@freehck.ru>
