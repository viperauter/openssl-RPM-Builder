# Сборка RPM OpenSSL версии 1.1.1d (для CentOS 7)


## Установка:

    sudo yum groupinstall 'Development Tools'

    cd /opt
    git clone https://github.com/philyuchkoff/openssl-1.1.1d-RPM-Builder.git
    cd openssl-1.1.1d-RPM-Builder/
    git checkout master

    make
    
Собранный RPM будет лежать в 

    /opt/openssl-1.1.1d-RPM-Builder/rpmbuild/RPMS/x86_64
    
## Проверка

После установки пакета можно проверить:

        openssl version
    
должно ответить так:

    OpenSSL 1.1.1d  28 May 2019