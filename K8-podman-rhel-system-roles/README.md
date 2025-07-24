You can use the podman RHEL system role to create rootless containers with bind mount by running an Ansible playbook and with that, manage your application configuration.

1. The playbook https://github.com/rnunezrgn/Kubernetes/blob/main/K8-podman-rhel-system-roles/configure-podman-bind-mount.yaml starts two Kubernetes pods: one for a database and another for a web application. The database pod configuration is specified in the playbook, while the web application pod is defined in an external YAML file.

2. The second https://github.com/rnunezrgn/Kubernetes/blob/main/K8-podman-rhel-system-roles/configure-rootful-container-with-podman-volume.yml playbook create a rootful container with a Podman volume by running an Ansible playbook and with that, manage your application configuration.

The example Ansible playbook deploys a Kubernetes pod named ubi8-httpd running an HTTP server container from the registry.access.redhat.com/ubi8/httpd-24 image. The container’s web content is mounted from a persistent volume named ubi8-html-volume. By default, the podman role creates rootful containers.

