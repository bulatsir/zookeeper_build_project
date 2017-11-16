# zookeeper_build_project
Для сборки потребуется установленный Vagrant (использовался 2.0.1), Virtualbox   и Ansible (использовался 1.5.4)

Описание файлов:

vagrantfile - файл c описанием окружения виртуальных машин для Vagrant
host - inventory файл для Ansible с описанием хостов
playbook.уml - файл для управления конфигурацией ВМ Ansible

Инструкция 

Поместить все файлы в необходимую директорию. 

Поднять окружение Vagrant (в директории должен находится файл vagrantfile):

vagrant up

Запустить сценарий сборки пакета:

ansible-playbook -i host playbook.yml -v 
