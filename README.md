# zookeeper_build_project
## Сборка deb пакета на ВМ Ubuntu 14* при помощи Ansible

Для сборки потребуется установленный Vagrant (использовался 2.0.1), Virtualbox   и Ansible (использовался 1.5.4)

### Описание файлов:

* vagrantfile - файл c описанием окружения виртуальных машин для Vagrant
* host - inventory файл для Ansible с описанием хостов
* playbook.уml - файл для управления конфигурацией ВМ Ansible

Поместить все файлы в необходимую директорию. 

Поднять окружение Vagrant (в директории должен находится файл vagrantfile):

_vagrant up_

Запустить сценарий сборки пакета:

_ansible-playbook -i host playbook.yml -v_
