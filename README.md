Это скрипт для зеркалирования сайтов и отслеживания изменений в них.

Необходимый сайт закачивается через wget в заранее созданный git-репозиторий,
скрипт сбрасывает все изменения в log и коммитит текущую версию.

Для работы скрипта первым аргументом необходимо подать адрес файла, в котором
через пробел записаны адреса сайтов и их локальных репозиториев. Последняя строка
обязаткльно должна содержать \n. Формат:

URL1 path1
URL2 path2
URL3 path3


Сам скрипт имеет смыл запускать через cron с определённой периодичностью.