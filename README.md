# ansible playbooks

* inventory/\*.yml has to have hosts otherwise nothing to do
* `files/00-id-rsa.pub` is used by `deb11/01-initialize.yml` for authing, if you don't add you might get locked out.

## Usage

```bash
# Fill out
ansible-playbook playbooks/deb11/00-initialize.yml -e "target_host= root_password= user_name= user_password="
ansible-playbook playbooks/deb11/01-update.yml
```