# Lab 3
## Хід роботи
1. Створив віртуальне середовище у папці Lab3 та встановив на неї усі необхідні пакети
            
       (Lab3) user@Pc:~/GitRepos/DevopsLabs/Lab3$ pipenv install django
       Installing django...
       Adding django to Pipfile's [packages]...
       ✔ Installation Succeeded 
       Pipfile.lock not found, creating...
       Locking [dev-packages] dependencies...
       Locking [packages] dependencies...
       Building requirements...
       Resolving dependencies...
       ✔ Success! 
       Updated Pipfile.lock (85c883)!
       Installing dependencies from Pipfile.lock (85c883)...
         🐍   ▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉▉ 0/0 — 00:00:00
       (Lab3) user@Pc:~/GitRepos/DevopsLabs/Lab3$ 
2. Створив заготовку сайту за допомогою Django Framework та виніс файли на рівень вище
        
       (Lab3) user@Pc:~/GitRepos/DevopsLabs/Lab3$ pipenv run django-admin startproject my_site
3. Запустив Django сервер за допомогою команди ```pipenv run python manage.py runserver```<br/>
![](photos/1.jpg)
4. Все запустилось успішно і стартова сторінка Django відображається коректно
5. Зупинив сервер через Ctrl-C та зробив коміт.
6. Cтворив темплейт свого додатку (app) у якому та закомітив ці файли до свого репозиторію.
        

