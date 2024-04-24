Task:
>a) Выполняется в локальной операционной системе.
Создать текстовый документ (sys.tat), в котором будет содержаться «Системная информация».
Написать программу-инсталлятор sys_doc.exe для этого документа, которая под видом установки обновления (с отображением строки прогресса обновления) к какой-нибудь программе (например, Блокнот или Paint):
Запрашивает у пользователя папку (должен быть вариант использования существующей папки и вариант создания собственной) для копирования «Системной информации».
Записывает в папку файл с исполняемым кодом программы secur.exe (аналог требований к template.tbl из лабораторной работы №1), защищающей sys.tat.
Собирает (возможную) информацию о компьютере, на котором устанавливается программа.
Кодирует эту информацию и записывает в файл sys.tat.
Подписывает её личным ключом пользователя программы и записывает подпись, например, в реестр Windows в раздел HKEY_CURRENT_USER\Software\Фамилия_студента как значение параметра Signature.
Запускает secur.exe для защиты sys.tat от несанкционированного доступа.
Прописывает запуск программы secur.exe при выполнении функции Open для sys.tat, чтобы защита срабатывала и после перезагрузки ОС (есть несколько способов такой «привязки»).
В саму программу защиты secur.exe включить следующий функционал:
Запрос у пользователя информации об имени раздела реестра с электронной цифровой подписью (фамилией студента).
Считывание подписи из указанного выше раздела реестра, которая проверяется с помощью открытого ключа пользователя.
Разрешение или запрет просмотра «Системной информации» в файле sys.tat в зависимости от правильности указания ключа.
При неудачной проверке работа защищаемой программы должна прекращаться с выдачей соответствующего сообщения.
Собираемая о компьютере информация включает в себя как минимум:
Имя пользователя,
Имя компьютера,
Конфигурацию компьютера (память и процессор, как минимум) и версию ОС.


>b)> Выполняется в локальной сети (или виртуальной).
 Создать скрипт, который удалённо и незаметно для пользователя (пользователь открывает какую-нибудь веб-страничку от создателя скрипта) собирает информацию о нём, его компьютере и системе (п.5 предыдущего задания) и записывает её на какой-либо локальный сетевой диск (доступный создателю скрипта) в папку с именем IP или Mac-адреса пользовательской машины.
Продумать доступ к этой информации (можно писать на удалённый диск).
Протестировать на 3-5 клиентах и получить статистику о них.
После демонстрации инсталлятора и скрипта исходники и документацию (в т.ч. расширенную инструкцию по применению) заархивировать и отправить на почту.
Приветствуется расширение функционала и оригинальные решения. Рекомендуется выполнять на виртуальной машине.