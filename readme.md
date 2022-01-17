## Play with ansible @ Hetzner

### Get a hetzner API Token and set the environment variable HCLOUD_TOKEN

```shell
export HCLOUD_TOKEN=xxxxxxxxxxxxxxxxxxxxxxxxxx
```

### Satisfy requirements for ansible (once)

```shell
pip install --user ansible
pip install --user hcloud
ansible-galaxy collection install --requirements-file requirements.yaml
ansible-galaxy role install --role-file requirements.yaml
```


```shell
ansible-playbook -vvv provision.yaml
```
