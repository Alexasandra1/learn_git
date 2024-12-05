# Введение
Надеюсь после первой задачи вы научились отслеживать изменения файлов, а так же коммитить изменения.

Valeriya_Penina
# Начинаем

Теперь давайте попробуем забрать из репозитория задачу выполненную другим разработчиком. В данном 
случае это будет очередной абзац нашего стихотворения

## Задание 

1. Из текущей ветки (dev-task_1) сознайте новую с именем состоящим из ваших ФИО, например *Vasia_Pupkin* это
   будет ваша основная ветка. От нее создайте еще одну ветку *task_1*
2. Добавьте в **index.html** первый абзац стихотворения
3. Выполните команду **git status**, обратите внимание на статус *modified* измененного файла
   Данный статус сообщает, что файл был изменен.
4. Создайте какой-либо файл и выполните **git status** еще раз, теперь вы должны увидеть,  
   что кроме *modified* git сообщает нам о *untracket files*, это означает, что этот файл   
   не отслеживается гитом
5. Добавьте ВСЕ изменения в коммит командой **git add -A**, выполните **git status**  
   обратите внимание, что все изменения готовы к коммиту *Changes to be committed*  
6. Внесите любую правку в свой тестовый, файл и проверьте статус **git status**,  
   теперь вы можете увидеть, что ваш файл отображается сразу в двух статусах.  
   Что бы добавить новые изменения к коммиту вам опять нужно выполнить **git add**  
   либо отменить ваши изменения командой **git checkout <nameFiles>** о чем вас проинформирует  
   консоль.  
   ***Важно отметить, что в коммит попадут только те изменения которые находятся в *staged* т.е.
   добавлены к коммиту. Очень важно контролировать изменения прикрепляемые к коммиту, так как 
   в него могут не попасть нужные изменения (вы забыли **git add**), либо попадут изменения 
   которых там быть не должно (например файлы пользователя)***
7. Попробуйте самостоятельно, добавлять файлы, вносить правки, добавлять к коммиту, сбрасывать изменения.
   Не бойтесь, что-либо сломать, это тренировка и она важна для понимания процессов.
8. Когда вы точно понимаете как управлять изменениями, создайте коммит **git commit** либо 
   **git commit -m <nameCommit>**, проверьте еще раз статус, там не должны отображаться изменения
   которые были добавленны к коммиту
9. Смержите основную ветку с веткой задачи, для этого перейдите в вашу основную ветку и выполните
   комманду git merge <name branch>, обязательно обратите внимание, что результатом вашего слияния
   стал новый коммит.
10. Отправьте ваши изменения в удаленный репозиторий **git push origin** где *origin* будет вашим

1. Из вашей основной ветки **name_surname**, создайте новую ветку **task_2** и перейдите в нее.
2. Выполните команду *git pull origin dev-task_2*. Вы заберете второй абзац стихотворения который
   имитирует задачу выполненную другим разработчиком.
3. В случае если у вас появились конфликты слияния, разрешите их.
4. Смержите ветку **task_2** с **name_surname**.
5. Результатом вашей работы должны быть 2 столбца стихотворения.
6. Отправьте ваши изменения в удаленный репозиторий **git push origin** где *origin* будет вашим

   удаленным репозиторием, сделайте pull request.


## Может понадобится
В результате работы у вас могут появляться файлы, которых не должно быть в репозитории
(например файлы среды разработки), для того что бы они не висели в *статусе* добавьте 
их в **.gitignore**. Просто создайте этот файл и запишите в нем файл или папку которы не должен
отслеживать git.

# Введение

Данный материал предназначен для введения в систему контроля версий GIT, и  
получению практики по базовым командам.

## Для работы Вам понадобится:
1. Aккаунт на github
2. Несколько часов свободного времени
3. Желание понять как начать работать с GIT 

## Порядок работы: 
1. Все задания вы выполняете в своем локальном репозитории
2. Каждая задача выполняется в новой ветке с именем *task_#*, где # - номер вашей задачи
3. Вашей основной веткой будет ветка с именем *name_surname*, например *Vasia_Pupkin*
4. После выполнения задачи вы мержите ветку *task_#* с веткой *name_surname* (если в задании
   не указано иного), синхронизируете ее со своим репозиторием на github, делаете pull request
   в репозиторий [sotbit/learn_git](https://github.com/sotbit/learn_git)
5. Каждая задача описана в соответствующей ветке, в файле README.md
6. Просмотреть вашу работу можно открыв index.html в любом браузере (после изменений не забывайте
   обновить браузер).

## Очень важно
Что бы все задачи не прошли мимо, нужно обязательно разобраться в том, что происходит.
Для этого:
1. ***Всегда*** смотрите файл на своей а так же учебной, до начала выполнения, в процессе и после 
   выполнения задачи.
2. Если вы что-то не понимаете, попробуйте разобраться самостоятельно, поищите информацию.
   Если это не помогает, обратитесь к наставнику. Не переходите к следующему заданию пока не разобрались
   с текущим.
3. Обязательно пробуйте сделать все что описано в задачах, ***НЕ копируйте текст***, введите 
   его руками, пробуйте изменять что-нибудь в файлах. Не бойтесь что-то сломать.
4. Не торопитесь скорее выполнить задания, все примеры **очень легкие**, весь курс можно сделать
   за 10 минут, но его ***задача что бы вы разобрались*** именно поэтому тут нет привязки к коду 
   или форматированию.
   
* А так же не забывайте разрешать конфликты в README.md

## Начинаем
1. Сделайте fork из репозитория [sotbit/learn_git](https://github.com/sotbit/learn_git)
2. Клонируйте репозиторий на вашу локальную машину
3. В вашем локальном проекте перейдите в ветку *dev-task_1*, что бы узнать ваше первое задание.

## Может понадобиться
* **git status** - проверить статус
* **git checkout name-branch** - переключает на ветку name-branch
* **git checkout -b name-branch** - создает ветку name-branch и переходит на нее
* **git branch** - отображает список доступных веток
* **git branch --all** - отображает список доступных веток в т.ч на удаленном репозитории
* **git pull** - забирает изменения и сливает ветки
* **git push** - отправляет изменения
* **git log --all --oneline --graph** - строит историю в консоли (попробовать обязательно)
master
