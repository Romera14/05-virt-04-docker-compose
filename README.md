# Домашнее задание к занятию 4. «Оркестрация группой Docker-контейнеров на примере Docker Compose» - Паромов Роман

## Задача 1

### Создайте собственный образ любой операционной системы (например ubuntu-20.04) с помощью Packer (инструкция).

Не понимаю откуда он берет образы. 
```
==> yandex: Creating temporary RSA SSH key for instance...
==> yandex: Error getting source image for instance creation: server-request-id = 7599f57a-5525-4c6b-807a-f5d7a5475523 server-trace-id = 2d9a0d0583337fc:37dee3ee938f07c0:2d9a0d0583337fc:1 client-request-id = 25eee99c-c1f3-4d53-8ace-da4f4408b9c4 client-trace-id = e3798c2d-15a3-462f-a01b-802c7a446a70 rpc error: code = NotFound desc = Image "centos-8" not found
Build 'yandex' errored after 15 seconds 852 milliseconds: Error getting source image for instance creation: server-request-id = 7599f57a-5525-4c6b-807a-f5d7a5475523 server-trace-id = 2d9a0d0583337fc:37dee3ee938f07c0:2d9a0d0583337fc:1 client-request-id = 25eee99c-c1f3-4d53-8ace-da4f4408b9c4 client-trace-id = e3798c2d-15a3-462f-a01b-802c7a446a70 rpc error: code = NotFound desc = Image "centos-8" not found
```

Чтобы получить зачёт, вам нужно предоставить скриншот страницы с созданным образом из личного кабинета YandexCloud.

## Задача 2

### 2.1. Создайте вашу первую виртуальную машину в YandexCloud с помощью web-интерфейса YandexCloud.

### 2.2.* (Необязательное задание)
Создайте вашу первую виртуальную машину в YandexCloud с помощью Terraform (вместо использования веб-интерфейса YandexCloud). Используйте Terraform-код в директории (src/terraform).

Чтобы получить зачёт, вам нужно предоставить вывод команды terraform apply и страницы свойств, созданной ВМ из личного кабинета YandexCloud.

## Задача 3

### С помощью Ansible и Docker Compose разверните на виртуальной машине из предыдущего задания систему мониторинга на основе Prometheus/Grafana. Используйте Ansible-код в директории (src/ansible).

Чтобы получить зачёт, вам нужно предоставить вывод команды "docker ps" , все контейнеры, описанные в docker-compose, должны быть в статусе "Up".

## Задача 4

### Откройте веб-браузер, зайдите на страницу http://<внешний_ip_адрес_вашей_ВМ>:3000.
Используйте для авторизации логин и пароль из .env-file.
Изучите доступный интерфейс, найдите в интерфейсе автоматически созданные docker-compose-панели с графиками(dashboards).
Подождите 5-10 минут, чтобы система мониторинга успела накопить данные.
Чтобы получить зачёт, предоставьте:

скриншот работающего веб-интерфейса Grafana с текущими метриками, как на примере ниже.


## Задача 5 (*)

### Создайте вторую ВМ и подключите её к мониторингу, развёрнутому на первом сервере.

Чтобы получить зачёт, предоставьте:

скриншот из Grafana, на котором будут отображаться метрики добавленного вами сервера.
