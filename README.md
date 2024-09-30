# Домашнее задание к занятию «Хранение в K8s. Часть 2» - Тертерян Вячеслав

---

### Задание 1  

Создать Deployment приложения, использующего локальный PV, созданный вручную.

1. Продемонстрировать, что multitool может читать файл, в который busybox пишет каждые пять секунд в общей директории  

Ответ:  
![alt text](https://github.com/Marsianec/homework23-7/blob/main/img/1.png)  

2. Удалить Deployment и PVC. Продемонстрировать, что после этого произошло с PV. Пояснить, почему.  

Ответ:  
PV перейдет в статус Released так как нет PVC и POD.  
![alt text](https://github.com/Marsianec/homework23-7/blob/main/img/2.png)  

3. Продемонстрировать, что файл сохранился на локальном диске ноды. Удалить PV. Продемонстрировать что произошло с файлом после удаления PV. Пояснить, почему.  

Ответ:  
Ну собсветнно что он остался на диске вот скрин  
![alt text](https://github.com/Marsianec/homework23-7/blob/main/img/2.png)  

И он так же останется и после удаления PV.  
![alt text](https://github.com/Marsianec/homework23-7/blob/main/img/3.png)  


Манифесты данного задания:  
![alt text](https://github.com/Marsianec/homework23-7/blob/main/img/4.png)  

---

### Задание 2  

Создать Deployment приложения, которое может хранить файлы на NFS с динамическим созданием PV.

Ответ:  

Скрин 1  
![alt text](https://github.com/Marsianec/homework23-7/blob/main/img/5.png)  

Скрин 2  
![alt text](https://github.com/Marsianec/homework23-7/blob/main/img/6.png) 