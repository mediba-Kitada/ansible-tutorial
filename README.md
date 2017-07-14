yatsushiro さんの課題
====

## 1. Ansible Playbookの不具合を修正してください。
- 対象のロールは、`wordpress`のみです。
	- `common`は正常に動作するので、考慮しなくてよいです。

## 2. Ansible PlaybookでWordpressサーバをプロビジョニングし、Wordpressの設定画面を表示してください。
- プロビジョニングコマンド
	- `$ ansible-playbook -i ./inventories/tech_lab --private-key=~/.ssh/wordpress site.yml`
- URLは、以下の通りです。
	- http://wordpress-serv-ELB-1V3W7P0MCCYZ-1527937663.ap-northeast-1.elb.amazonaws.com/wp-admin/install.php
- Ansible Playbookの不具合を修正しないと設定画面は、表示されません。

## 修正内容をコミットし、Pull Requestしてください。
- 作業ブランチは、`fix/yatsushiro`としてください。
	- `$ git checkout -b fix/yatsushiro`
- PR対象のブランチは、`yatsushiro`としてください。
	- `$ git pull-request -m 'Ansible入門 yatsushiro' -b yatsushiro`
