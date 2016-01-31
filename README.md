[![Build Status](https://travis-ci.org/ike-jp/ansible-role-vim.svg?branch=master)](https://travis-ci.org/ike-jp/ansible-role-vim)

Ansible Role: Vim
=========

Under development

Requirements
------------

+ RedHat/CentOS: git
+ Debian/Ubunt: git


Role Variables
--------------

Available variables are listed below, along with default values (see defaults/main.yml):

```yaml
vim_repository_url: https://github.com/vim-jp/vim.git
vim_installation_version: v7.4.393
vim_installation_dir: $HOME/ansible_test/local
vim_installation_src_dir: ~/ansible_test/tmp/vim

vim_configures_to_build:
  - --with-features=huge
  - --enable-multibyte
  - --enable-fail-if-missing
  - --enable-pythoninterp
...

```


Dependencies
------------

+ None.

If install interpreter by anyenv,
for example you will need the following roles.

+ ike-jp.anyenv
+ yaegashi.blockinfile


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

```yaml
    - hosts: servers
      roles:
         - { role: ike-jp.vim }
```


License
-------

MIT License


Author Information
------------------

This role was created in 2016 by ike-jp.




[![Bitdeli Badge](https://d2weczhvl823v0.cloudfront.net/ike-jp/ansible-role-vim/trend.png)](https://bitdeli.com/free "Bitdeli Badge")

