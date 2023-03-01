1. создать ssh
ssh-keygen -t ed25519 -C "your_email@example.com"
> Generating public/private ed25519 key pair.
> Enter a file in which to save the key (/Users/you/.ssh/id_ed25519): [Press enter]
> Enter passphrase (empty for no passphrase): [Press enter]
> Enter same passphrase again: [Press enter]
eval "$(ssh-agent -s)"
> Agent pid 59566
$ ssh-add ~/.ssh/id_ed25519
2. добавление публичного на гитхаб
Скопируйте содержание файла SSH ключа в буфер обмена
Вставьте в гитхаб
3.как склонировать реп
git clone git@github.com:username/repository.git