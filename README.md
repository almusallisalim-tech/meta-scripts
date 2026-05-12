---
# meta-scripts 🚀

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
```
```bash
git clone https://github.com/USERNAME/meta-scripts.git
cd meta-scripts
docker run -it -v $(pwd):/work ubuntu:22.04 bash
cd /work
apt update && apt install -y ansible
ansible-playbook test.yml
```
```yaml
---
- hosts: localhost
  connection: local
  tasks:
    - name: ترحيب
      debug:
        msg: "Ansible شغال بدون dpkg 🎉"
```
*1.* `Add file` > `Create new file`  
*2.* الاسم: `test.yml`  
*3.* 

*الوضع الحالي:*
العنصر	الحالة
**README.md**	✅ كامل ومضبوط
**الأوامر**	✅ `apt` صحيحة
**بلوك YAML**	✅ ملون ومرتب
**ملاحظة UserLand**	✅ أسطورية 😂

*4.* `Commit new file`


## ملاحظة
هذا المشروع كان لحل مشكلة `dpkg-statoverride` على UserLand 😂  
الحل النهائي: Do
