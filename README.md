# Парсинг контента ВКонтакте

Python парсер, который позволяет брать разные посты из групп ВК и добавлять в свою группу.

## Настройка
Для начала работы необходимо открыть config.py и сделать следующее:

1. Указать `ownerId_wallPost` - ID своей группы;
2. Получить `VK_ACCESS_TOKEN`. Вот тут - https://vkhost.github.io/
3. Перечислите группы, из которых будет забираться контент в списке `vk_group`;
4. Перечислить "стоп" слова при которых пост не будет опубликован в списке `stop_list`
5. Перечислить слова, которые будут удалены из поста, если они там будут в списке `blacklist`
6. При необходимости заменить watermark.png

Готово. Теперь посты из других групп будут добавляться в вашу. В файле настроек (`config.py`) есть различные опции с описанием их работы. Вы можете изменить их под ваши нужды.
### Если не будет работать, то выполните следующие шаги:
1. Установите зависимости - `pip install -r requirements.txt`
2. Проверить наличие директории `temp_img` в корне проекта
3. Убедитесь что у вас стоит Python 3(скрипт разрабатывается на Python 3.8.10)