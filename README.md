# Tesst for phoenix55rus

взять чистую виртуальную машину в virtualbox на ubuntu 18.04, написать плейбук ansible который делает следующее:
 - ставит nginx, zsh, wget
 - клонирует из git в /var/www/ очень простую  web страничку "Under construction"
 - кладет новую конфигурацию nginx которая направляет на эту страничку
 - настраивает в sysctl параметр fs.files-max в 1204000 и somaxconn в 65535
 - прописывает на этой машинке 2 разных ssh ключа в /root
 - результат в git на github в приватном репозитории

Считаем, что код не “одноразовый” и будет использоваться командой для управления виртуальной машиной и далее.