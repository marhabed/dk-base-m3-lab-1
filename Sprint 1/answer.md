# Sprint 1
TODO: Student to complete code and comments in the sections below.

## Install Kubernetes node 1

- Customized kubeadm-config.yaml:
- apiVersion: v1
clusters:
- cluster:
    certificate-authority-data: LS0tL...tLS0K
    server: https://172.31.35.56:6443
  name: kubernetes
contexts:
- context:
    cluster: kubernetes
    user: kubernetes-admin
  name: kubernetes-admin@kubernetes
current-context: kubernetes-admin@kubernetes
kind: Config
preferences: {}
users:
- name: kubernetes-admin
  user:
    client-certificate-data: LS0t...S0tCg==
    client-key-data: LS0t...tLS0tCg==
