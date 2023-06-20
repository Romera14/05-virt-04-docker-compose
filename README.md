# Домашнее задание к занятию 4. «Оркестрация группой Docker-контейнеров на примере Docker Compose» - Паромов Роман

## Задача 1

### Создайте собственный образ любой операционной системы (например ubuntu-20.04) с помощью Packer (инструкция).

![](https://github.com/Romera14/05-virt-04-docker-compose/blob/main/Снимок%20экрана%202023-06-21%20в%2001.14.14.png)
![](https://github.com/Romera14/05-virt-04-docker-compose/blob/main/Снимок%20экрана%202023-06-21%20в%2001.21.00.png)

Чтобы получить зачёт, вам нужно предоставить скриншот страницы с созданным образом из личного кабинета YandexCloud.

## Задача 2

### 2.1. Создайте вашу первую виртуальную машину в YandexCloud с помощью web-интерфейса YandexCloud.

![](https://github.com/Romera14/05-virt-04-docker-compose/blob/main/Снимок%20экрана%202023-06-21%20в%2001.25.48.png)

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
