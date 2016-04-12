# test-ansible-roles
## 概要
- win10 + Vagrant(1.8.1) + CentOS6.7 + ansible_local
- ansible_local(インストールされるバージョンは指定不可)
- ansibleの雛型フォルダを空登録
- 様々な role のテスト・保存用
```
$ cd provisioning/roles/common
$ ls | xargs -t -I{} touch {}.gitkeep
```
- playbookテスト
```
[vagrant@test-rails01 ~]$ cd /vagrant/provisioning
[vagrant@test-rails01 provisioning]$ ansible-playbook -i hosts/test test.yml
```
## ロール
- nvm
- rbenv

