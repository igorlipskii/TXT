 1. Создать внешний репозиторий c названием TXT.\
нажать `+` `New repository`

 2. Клонировать репозиторий TXT на локальный компьютер.\
`cd /Users/igori/Documents/github`\
`git clone https://github.com/igorlipskii/txt.git`

 3. Внутри локального TXT создать файл “new.txt”.\
`touch new.txt`

 4. Добавить файл под гит.\
`git add new.txt`\
`git status`

 5. Закоммитить файл.\
`git commit -m "add new file"`

 6. Отправить файл на внешний GitHub репозиторий.\
`git push`

 7. Отредактировать содержание файла “new.txt” - написать информацию о себе (ФИО, возраст, количество домашних животных, будущая желаемая зарплата). Всё написать в формате TXT.\
`vim new.json`\
`i` — перейти в режим редактирования

```txt
Name: Igor Lipskii
Age: 33
Pet: no pets
Salary: 
    1. Junior - 80.000 rub. 
    2. Middle - 190.000 rub.
    3. Senior - 320.000+ rub.
```
`esc` `:` `wq`

 8. Отправить изменения на внешний репозиторий.\
`git add new.txt`\
`git commit -m  "wrote information about myself"`\
`git push`

 9. Создать файл preferences.txt\
`touch preferences.txt`

 10. В файл preferences.txt” добавить информацию о своих предпочтениях (Любимый фильм, любимый сериал, любимая еда, любимое время года, сторона которую хотели бы посетить) в формате TXT.\
`vim preferences.txt`\
`i` — перейти в режим редактирования

```txt
My preferences:
	Film: John Carter
	Series: La casa de papel
	Food: pasta, vegetables and meat
	Season: Summer
	Place to visit: USA, Japan, New Zealand
```
`esc` `:` `wq`

 11. Создать файл sklls.txt добавить информацию о скиллах которые будут изучены на курсе в формате TXT\
`vim skills.txt`\
`i` — перейти в режим редактирования

```txt
Skills:
        1. Basic theory (What is testing, bug reports, documentation, types, methods, testing directions, etc.).
        2. What is a client-server architecture.
        3. HTTP Methods of requests to the server.
        4. HTTP server response codes.
        5. Structures of HTTP requests and responses.
        6. What is JSON, XML. Their structure.
        7. API testing via Postman (JS, API autotests).
        8. Removing and reading logs from an external server.
        9. Sniffing http web traffic via Charles and Fiddler.
        10. Dev Tools of web browsers (Google Chrome, FireFox).
        11. VPN (How it works, why you need it, how to use it, tool options).
        12. Mobile testing.
        13. Feature iOS, Android, guidelines.
        14. Building iOS applications on XCode. (Those who do not have a Mac computer, just look).
        15. Building Android applications on Android Studio.
        16. ADB (android device management).
        17. Setting up proxy and vpn on iOS and Android.
        18. Interception (sniffing) of mobile traffic via Charles and Fiddler on iOS and Android.
        19. "Command line (terminal) Linux (copying, creating, viewing, moving files on servers without a graphical interface).
        20. "Basics of bash scripting, automation of routine tasks on the server.
        21. "Access to remote servers.
        22. "SQL basics (Create, Delete, Drop, Insert Into, Select, From, Where, Join).
        23. "Postgres database (installation, configuration and use).
        24. "Non-relational database Redis (installation, configuration and use).
        25. "Load testing in Jmeter.
        26. "Scrum development methodology.
        27. "Python. (Learning the basics. Creating a client-server application).
```
`esc` `:` `wq`

 12. Сделать коммит в одну строку.\
`git add {preferences,skills}.txt && git commit -m "add and commit 2 files"`

 13. Отправить сразу 2 файла на внешний репозиторий.\
`git status`\
`git push`

 14. На веб интерфейсе создать файл bug_report.txt.\
нажать `add new file` `create new file` пишем название файла

 15. Сделать Commit changes (сохранить) изменения на веб интерфейсе.\
в `commit new file` пишем `create bug_report`

 16. На веб интерфейсе модифицировать файл bug_report.txt, добавить баг репорт в формате TXT.\
нажать `edit this file`

```txt
Project: Calculator
ID: 88
Summary: Результат умножения неверен
Description: Результат равен ожидаемому результату +2
    Steps to reproduce:
    Step 1: Открыть сайт https://nuix.github.io/SDET/senior-sdet/stagingCalc/index.html
    Step 2: Нажать цифру 6
    Step 3: Нажать знак умножения
    Step 4: Нажать цифру 3
    Step 5: Нажать знак равно
Actual result: 20
Expected result: 18
Attachments: https://somup.com/c3nq02TjpH
Severity: Critical
Priority: High
Labels: Smoke
Environment:
Operational system: macOS Big Sur 11.6.4
Browser version: Google Chrome 98.0.4758.102
Author: Igor Lipskii
Test Data: 20.02.2022
```
 17. Сделать Commit changes (сохранить) изменения на веб интерфейсе.\
пишем в `Commit changes` `update bug_report`
 18. Синхронизировать внешний и локальный репозиторий TXT\
`git pull`