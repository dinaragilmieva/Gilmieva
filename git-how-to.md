Чтобы создать ssh ключ на Git Bush:
1. Проверяем, есть ли у нас уже созданный ключ: ls ~/.ssh
2. Создаем ключ: ssh-keygen -t ed25519 -C "dinaragilmieva@mail.ru"
3. Выводим значение ключа: cat ~/.ssh/id_ed25519.pub

Добавляем ключ на GitHub:
1. Открываем github
2. Settings
3. SSH and GPG keys
4. New SSH key
5. В поле Key вставляем публичный ключ из Git Bush (cat ~/.shh/id_ed25519.pub)
6. Add SHH key
7. Провряем ключ в Git Bush: shh -T git@github.com

Rлонируем репризиторий:
1. git clone <адрес репризитория>
