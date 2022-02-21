# XML
##### 1. Создать внешний репозиторий c названием XML.

перейти на сайт `https://github.com.` Залогиниться. Нажать кнопку` New`.

в поле `Repository name` ввести XML, выбрать `Public` и `Add a README file`.

Нажать `Create repository.`

##### 2. Клонировать репозиторий XML на локальный компьютер.

Нажать `Code`, выбрать HTTPS, скопировать ссылку на репозиторий,

на локальном компьютере  зайти в папку(в которой будет размещен репозиторий), запустить  gitbash 

`git clone https://github.com/zhuravskaya-anna/XML.git`

`cd XML` (переходим в папку XML (в конце адреса указано имя ветки  main )

##### 3. Внутри локального XML создать файл “new.xml”.

 `touch new.xml`

##### 4. Добавить файл под гит.

`git status` - проверить статус название файла  отображается красным (изменения в файле не отслеживаются) 

`git add` . -Эта команда добавит файл в раздел проиндексированных файлов Git (начинается отслеживание измений в файле)

`git status` - проверить статус Окрашенный зеленым цветом вывод «new file: сообщает о том, что файл  будет сохранен при выполнении следующего коммита   (изменения в файле отслеживаются)

##### 5. Закоммитить файл.

`git commit -m "new file xml"`

##### 6. Отправить файл на внешний GitHub репозиторий.

`git push`  выгружаем содержимое локального репозитория в удаленный репозиторий


##### 7. Отредактировать содержание файла “new.xml” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате XML.


`vim new.xml `   воспользуемся встроенным редактором VIM открывается редактор
`i` команда insert, вход в режим редактирования

          <?xml version = "1.0"?>
          <aboutme>
            <person>
              <name>Ganna</name>
              <surname>Zhuravskaja</surname>
              <age>28</age>
            </person>
            <pets>
              <number>1</number>
                 <kind_of_pet>cat</kind_of_pet>
                 <name>Salvador</name>
              <number>2</number>						
                 <kind_of_pet>snail</kind_of_pet>
                 <name>Lusinda</name>
            </pets>
            <desiredSalary>500</desiredSalary>
          </aboutme>

`Esc`
`:wq`  сохранить и выйти

##### 8. Отправить изменения на внешний репозиторий.

`git commit -am "add info  new.xml"`  команда -am  аналогична запуску двух команд: git add для всех файлов, которые существовали в предыдущем коммите, и git commit с комментарием add info  new.xml

`git push`  выгружаем содержимое локального репозитория в удаленный репозиторий



##### 9. Создать файл preferences.xml

`cat > preferences.xml` используем команду cat > для создания  и добавления информации в фойл непосредственно в консоли

##### 10. В файл preferences.xml добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате XML.

          <?xml version = "1.0"?>
          <preferences>
            <favorite_movie>Men in Black</favorite_movie>
            <favorite_series>Downton Abbey</favorite_series>
            <favorite_food>Pasta</favorite_food>
            <favorite_season>spring</favorite_season>	
            <country_you_would_like_to_visit>Brazil</country_you_would_like_to_visit>
          </preferences>

`Ctrl + с`  сохранить и выйти из редактирования

#####  11. Создать файл sklls.xml добавить информацию о скиллах которые будут изучены на курсе в формате XML


`vim skills.xml`    воспользуемся встроенным редактором VIM открывается редактор
`i` команда insert, вход в режим редактирования

          <?xml version = "1.0"?>

          <skills>
            <theory>SDLC_STLC_Test_documentation_Types_of_testing</theory>
            <testing_tools>Postman_Charles_Fiddler_Jmeter</testing_tools>
            <database>SQL_PostgreSQL_DBeaver</database>
            <mobile_testing>Android_Studio_ADB</mobile_testing>
            <programming_language>Python</programming_language>
          </skills>
        

`Esc`
`:wq ` сохранить и выйти



##### 12. Сделать коммит в одну строку.
`git add . ; git  commit -m "add  files preference skill" `  для выполнения нескольких команд подряд используется  символ ;

##### 13. Отправить сразу 2 файла на внешний репозиторий.

` git push`

##### 14. На веб интерфейсе создать файл bug_report.xml.

Войти в репозиторий `XML`. Нажать кнопку` Add file.`

Выбрать `Create new file`. В поле `Name your file` ввести `bug_report.xml`

##### 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.


Нажать кнопку `Commit new filе` в нижней части экрана



##### 16. На веб интерфейсе модифицировать файл bug_report.xml, добавить баг репорт в формате XML.

Открыть файл bug_report.xml Выбрать  `Edit this file`. Ввести текст

          <?xml version = "1.0"?>
          <bug_report>
            <id>1</id>
            <Summary>Header->меню-> не верно назван элемент  Академия </Summary>
            <Severity>Minor</Severity>
            <Priority>Medium</Priority>
            <Environment>Windows 7 Professional 64-bit Google Chrome</Environment>
            <Description>в заголовке сайта в меню  Block-4 не верно назван элемент указано  Главная  вместо  Академия</Description>
            <Preconditions>User is on https://itcareer.pythonanywhere.com</Preconditions>
            <STR>Запустить браузер. перейти  https: АДРЕС. в заголовке сайта изучить название  элементов меню. сравнить со спецификацией</STR>
            <ER>элемент   Академия</ER>
            <AR>элемент Главная </AR>	
          </bug_report>



##### 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.

Нажать кнопку `Commit new filе` в нижней части экрана

##### 18. Синхронизировать внешний и локальный репозиторий XML

`git pull` используется для извлечения и загрузки содержимого из удаленного репозитория и немедленного обновления локального репозитория этим содержимым

