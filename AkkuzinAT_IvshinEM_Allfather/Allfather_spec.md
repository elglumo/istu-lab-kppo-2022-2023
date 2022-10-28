## Название проекта
Allfather

## Краткое описание сути проекта
Discord-бот для воспроизведения музыки в голосовых каналах Discord.

## Цель
Обеспечение возможности коллективного прослушивания музыки в голосовых каналах Discord.

## Аналитический обзор
Характеристика  | Hydra | MEE6 | Yukikaze | Gusic | Allfather |
----------------|-------|------|----------|-------|----------|
Проигрывать музыку с Youtube | нет | да | да | да | да |
Отедельный текстовый канал | да | нет | нет | нет | да | да |
Музкальная очередь | да | да | нет | нет | да |
Интерактивное отображение очереди | да | нет | нет | нет | да |
Включение музыки без спец. команды | да | нет | нет | нет | да |
Умное включение в голосовой канала | да | нет | да | нет | да |
Управление очередью треков | да | нет | нет | нет | да |
Количество реплик приложения | 6 | 12 | 6 | 6 | 1 |

## Результаты проекта
Реализация в виде серверного приложения.

### Функциональные требования
1. создание отдельного текстового канала при подключении бота к серверу;
2. воспроизведение аудиодорожки с Youtube по ключевому слову;
3. воспроизведение аудиодорожки с Youtube по прямой ссылке;
4. обрабатывание музыкальных запросов происходит только в рамках отдельно созданного текстового канала;
5. добавление трека в конец очереди, если сейчас ещё играет предыдущий трек;
6. специальная команда для перехода к следующему в очереди треку;
7. очистка очереди треков специальной командой;
8. перед началом воспроизведения трека бот добавляется в канал автора музыкального запроса;
9. если очередь пуста, то бот выходит из голосового канала;
10. интерактивно отображает текущую очередь треков;

## Допущения и ограничения
### Допущения
* допускается, что API Discord будет доступно и не изменится за всё время существования проекта;
* допускается, что API Youtube будет доступно и не изменится за всё время существования проекта;

### Ограничения
* интеграция исключительно с Discord;
* воспроизведение аудиодорожек исключительно с Youtube;