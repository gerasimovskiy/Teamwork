﻿1. Делаем копию общего репозитория в ваш GitHub аккаунт.
Для этого в общем репозитории нажимаем кнопочку Fork в правом верхнем углу.

2. Запускаем Git Bash и заходим в рабочую папку на своем компютере.
cd [путь в рабочую папку]

3. Клонируем свою копию удаленного репозитория на компьютер.
git clone [url вашего репозитория на GitHub]

4. В index.html находим свои разделы и там творим свою часть страницы.
Якоря в ваших разделах не трогайте.
Для стилей используем css-файл с вашим именем в папке css.
Используем font-family: 'roboto'. Из font.css берем font-weight и font-style.
Картинки из макета я сохранила в img. Если какие-то еще будете использовать, сохраняйте там же.
У кнопочек-ссылок на menu ставим href="menu.html".
Один из элемнтов должен иметь цвет #fffdc9

	<header></header>						- lnikolaenko
	<section class="welcome"></section>		- jeniatrofimenko
	<section class="about"></section>		- jeniatrofimenko
	<section class="food"></section>		- deni
	<section class="gallery"></section>		- deni
	<section class="contact"></section>		-  
	menu.html  								- ashmitya

5. Если что-то не получается и нужна помощь, отправляем файлы в свой репозиторий и пишем о проблеме в slack.
git add .
git commit -m "комментарии"
git push origin master

6. Когда все сделали, так же отправляем файлы в свой репозиторий и пишем в slack, 
нужно будет посмотреть не возникнет ли конфликтов в названии селекторов.

7. Когда получили добро, делаем Pull request на своей страничке на GitHub.

8. После того, как на общем репозитории все работы будут объединены, можно загрузить конечный результат 
к себе на компьютер и в свой репозиторий на GitHub.

В начале делаем привязку к общему репозиторию.
git remote add upstream https://github.com/LiudmilaNikolaenko/Teamwork

А потом стягиваем файлы на компьютер
git pull upstream master

и отправляем их в свой репозиторий на GitHub
git push origin master
