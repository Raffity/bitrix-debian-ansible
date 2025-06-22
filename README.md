# bitrix-debian-ansible
Bitrix setup for Debian 12 


## Установить ansible
Для windows удобнее использовать wsl

`apt install ansible`

Сгенерировать ssh ключ

`ssh-keygen -t rsa -i ansible -C "your_email@example.com"`

Скопировать на удаленный сервер

`ssh-copy-id -i ansible.pub -o "IdentityFile hostkey.rsa" user@target`

Запуск плейбука

`ansible-playbook -i inventory.ini site.yml`