You can use the podman RHEL system role to create rootless containers with bind mount by running an Ansible playbook and with that, manage your application configuration.

The playbook https://github.com/rnunezrgn/Kubernetes/blob/main/K8-podman-rhel-system-roles/configure-podman-bind-mount.yaml starts two Kubernetes pods: one for a database and another for a web application. The database pod configuration is specified in the playbook, while the web application pod is defined in an external YAML file.
