                                            ---
-# meta-scripts 🚀

مجموعة سكربتات Ansible للتجربة والتعلم على Docker

## المتطلبات
- Docker
- Ubuntu 22.04
- Ansible

## طريقة التشغيل
```bash
# 1. شغل container
docker run -it ubuntu:22.04 bash

# 2. ثبت Ansible
apt update && apt install -y ansible

# 3. شغل الـ playbook
ansible-playbook test.yml
```bash
