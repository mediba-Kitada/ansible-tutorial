m-sugimoto さんの課題
====

## 1. Ansible Playbookの不具合を修正してください。
- 対象のロールは、`wordpress`のみです。
	- `common`は正常に動作するので、考慮しなくてよいです。

## 2. Ansible PlaybookでWordpressサーバをプロビジョニングし、Wordpressの設定画面を表示してください。
- プロビジョニングコマンド
	- `$ ansible-playbook -i ./inventories/tech_lab --private-key=~/.ssh/wordpress site.yml`
- URLは、以下の通りです。
	- http://wordpress-serv-ELB-KWCTCJXU4FU0-235959442.ap-northeast-1.elb.amazonaws.com/wp-admin/install.php
- Ansible Playbookの不具合を修正しないと設定画面は、表示されません。

## 修正内容をコミットし、Pull Requestしてください。
- 作業ブランチは、`fix/m-sugimoto`としてください。
	- `$ git checkout -b fix/m-sugimoto`
- PR対象のブランチは、`m-sugimoto`としてください。
	- `$ git pull-request -m 'Ansible入門 m-sugimoto' -b m-sugimoto`
