# Домашнее задание к занятию "`Практическое применение Docker`" - `Ли Олег`


### Инструкция по выполнению домашнего задания

   1. Сделайте `fork` данного репозитория к себе в Github и переименуйте его по названию или номеру занятия, например, https://github.com/имя-вашего-репозитория/git-hw или  https://github.com/имя-вашего-репозитория/7-1-ansible-hw).
   2. Выполните клонирование данного репозитория к себе на ПК с помощью команды `git clone`.
   3. Выполните домашнее задание и заполните у себя локально этот файл README.md:
      - впишите вверху название занятия и вашу фамилию и имя
      - в каждом задании добавьте решение в требуемом виде (текст/код/скриншоты/ссылка)
      - для корректного добавления скриншотов воспользуйтесь [инструкцией "Как вставить скриншот в шаблон с решением](https://github.com/netology-code/sys-pattern-homework/blob/main/screen-instruction.md)
      - при оформлении используйте возможности языка разметки md (коротко об этом можно посмотреть в [инструкции  по MarkDown](https://github.com/netology-code/sys-pattern-homework/blob/main/md-instruction.md))
   4. После завершения работы над домашним заданием сделайте коммит (`git commit -m "comment"`) и отправьте его на Github (`git push origin`);
   5. Для проверки домашнего задания преподавателем в личном кабинете прикрепите и отправьте ссылку на решение в виде md-файла в вашем Github.
   6. Любые вопросы по выполнению заданий спрашивайте в чате учебной группы и/или в разделе “Вопросы по заданию” в личном кабинете.
   
Желаем успехов в выполнении домашнего задания!
   
### Дополнительные материалы, которые могут быть полезны для выполнения задания

1. [Руководство по оформлению Markdown файлов](https://gist.github.com/Jekins/2bf2d0638163f1294637#Code)

---

### Задание 3

![image](https://github.com/user-attachments/assets/f1c447c4-e69b-45a4-be9c-03a5bc78c4ac)




### Задание 4

![image](https://github.com/user-attachments/assets/803a0499-aa8e-4a42-bc53-59b01756122b)

```
#!/bin/bash
REPO_URL="https://github.com/ELK23/shvirtd-example-python"
TARGET_DIR="/opt/вshvirtd-example-python"
ENV_FILE=".env"
echo "Клонирование репозитория..."
if [ ! -d "$TARGET_DIR" ]; then
    git clone "$REPO_URL" "$TARGET_DIR"
else
    echo "Репозиторий уже существует. Обновляем..."
    cd "$TARGET_DIR" || exit
    git pull
fi
cd "$TARGET_DIR" || exit
echo "Запуск проекта..."
docker compose up -d
echo "Проверка состояния контейнеров..."
docker compose ps
```
https://github.com/ELK23/shvirtd-example-python

### Задание 6
![image](https://github.com/user-attachments/assets/1fcc37d9-3501-4dc3-98b5-c49a5902ebdb)

![image](https://github.com/user-attachments/assets/a671e191-9adf-4df4-bcb9-45038b54398a)

![image](https://github.com/user-attachments/assets/7e7c7370-cc5b-4df0-b337-035716340672)

![image](https://github.com/user-attachments/assets/7005cbd3-4677-4172-90f7-50694154109b)


![image](https://github.com/user-attachments/assets/128692f8-7366-4ded-bd72-9fede147358f)




### Задание 6.1
![image](https://github.com/user-attachments/assets/3bd4f243-91c8-460a-ae45-cef86e790d1b)

![image](https://github.com/user-attachments/assets/bd6e7a0e-21b1-48bf-ad3e-73e335909d3c)











