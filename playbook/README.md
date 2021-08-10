# Самоконтроль выполненения задания

1. Где расположен файл с `some_fact` из второго пункта задания?
    ansible-homeworks/01-base/ansible-base/playbook/group_vars/all/examp.yml
2. Какая команда нужна для запуска вашего `playbook` на окружении `test.yml`?
    ansible-playbook -i inventory/test.yml site.yml --vault-password-file secret.yml
3. Какой командой можно зашифровать файл?
    ansible-vault encrypt some_file.yml
4. Какой командой можно расшифровать файл?
    ansible-vault decrypt some_file.yml
5. Можно ли посмотреть содержимое зашифрованного файла без команды расшифровки файла? Если можно, то как?
    Нет
6. Как выглядит команда запуска `playbook`, если переменные зашифрованы?
    Например, так ansible-playbook -i inventory/test.yml site.yml --vault-password-file secret.yml
    Или так ansible-playbook -i inventory/test.yml site.yml --ask-vault-pass
7. Как называется модуль подключения к host на windows?
    winrm
8. Приведите полный текст команды для поиска информации в документации ansible для модуля подключений ssh
    ansible-doc -t connection ssh
9. Какой параметр из модуля подключения `ssh` необходим для того, чтобы определить пользователя, под которым необходимо совершать подключение?
    remote_user
