dit003 さんの課題
====

## 1. Ansible Playbookの不具合を修正してください。
- 対象のロールは、`wordpress`のみです。
	- `common`は正常に動作するので、考慮しなくてよいです。

## 2. Ansible PlaybookでWordpressサーバをプロビジョニングし、Wordpressの設定画面を表示してください。
- プロビジョニングコマンド
	- `$ ansible-playbook -i ./inventories/tech_lab --private-key=~/.ssh/wordpress site.yml`
- URLは、以下の通りです。
	- http://wordpress-serv-ELB-2UF6PXTXMNQ3-1101544215.ap-northeast-1.elb.amazonaws.com/wp-admin/install.php
- Ansible Playbookの不具合を修正しないと設定画面は、表示されません。

## 修正内容をコミットし、Pull Requestしてください。
- 作業ブランチは、`fix/dit003`としてください。
	- `$ git checkout -b fix/dit003`
- PR対象のブランチは、`dit003`としてください。
	- `$ git pull-request -m 'Ansible入門 dit003' -b dit003`
