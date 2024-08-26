Для реализации указанного приложения на языке Java, создадим программу, которая будет:

Запрашивать данные у пользователя.
Проверять количество введенных данных.
Выполнять парсинг и проверку форматов.
Обрабатывать возможные исключения.
Записывать данные в файл.
Объяснение программы:
Ввод данных:

Программа считывает строку, введенную пользователем, и разделяет ее на части по пробелу с помощью метода split(" ").
Проверка количества данных:

Проверяется, что введено ровно 6 элементов. Если их больше или меньше, выбрасывается исключение IllegalArgumentException с соответствующим сообщением.
Парсинг и проверка форматов:

Дата рождения проверяется регулярным выражением на соответствие формату dd.mm.yyyy.
Номер телефона должен быть числом, без каких-либо символов.
Пол должен быть либо f, либо m.
Обработка исключений:

Если происходит ошибка в количестве данных или формате, программа ловит IllegalArgumentException и выводит сообщение об ошибке.
Если возникает ошибка при записи в файл (например, из-за проблем с доступом к файлу), ловится IOException.
Запись в файл:

Данные записываются в файл с именем, равным фамилии пользователя. Если файл уже существует, новые данные добавляются в него на новой строке.
