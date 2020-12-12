# Lab 4
## Хід роботи
1. Ознайомився що таке Docker та документацією до нього;
2. Для перевірки, чи ```docker``` встановлено на моїй поточній машині, запустив почергово наступні команди та перенаправив їх у файл ```my_work.log```:
        
       docker -v >> my_work.log
       docker -h >> my_work.log
       docker run docker/whalesay cowsay Docker is fun >> my_work.log
   Зробив коміт з усіма змінами до репозиторію
3. Ознайомився з базовими принципами роботи ```docker``` та перейшов до виконання наступних пунктів.
4. Створив імедж із Django сайтом зробленим у попередній роботі:
    * Використав команду щоб завантажити базовий імедж з репозиторію:
            
          docker pull python:3.6-slim
          docker images
          docker inspect python:3.6-slim
          
          user@Pc:~/GitRepos/DevopsLabs/Lab4$ docker images
          REPOSITORY          TAG                 IMAGE ID            CREATED             SIZE
          python              3.6-slim            7fcd5f355774        22 hours ago        111MB
          docker/whalesay     latest              6b362a9f73eb        5 years ago         247MB
    * Створив файл з іменем Dockerfile скопіював туди вміст файлу з основного репозиторію;
    * Ознайомився із коментарями та зрозумів структуру написання Dockerfile;
    * Замінив посилання на власний Git репозиторій із моїм веб-сайтом та закомітив даний Dockerfile     