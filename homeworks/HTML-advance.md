
# Задания по теме "Продвинутый HTML" (Практика 3)

Каждое выполненное задание (все его файлы) заливается в репозиторий учащегося в отдельную директорию, после чего в файле README.md ставится ссылка на выполненное задание к соответствующему уроку.

Написанный код должен быть 100% валидным HTML5, т.е. ни одна из страниц не должна содержать ошибок и предупреждений при проверке через [W3 валидатор](https://validator.w3.org).

## Задание 1. Соцсеть фотографий и видео (Instagram)

### Техзадание

Сервис состоит из 3 страниц: главной страницы *index.html*, страницы ленты *feed.html* и страницы создания нового поста *photo-add.html*

На **главной странице** есть следующие блоки:

1. Название и логотип сервиса (header)
2. Форма входа (email и пароль - все поля обязательны)
3. Форма регистрации (имя на сервисе, email, пароль, подтверждение пароля, отметка о согласии с порядком обработки персональных данных - все поля обязательны)

После отправки любой формы пользователь попадает на страницу ленты.


**Страница ленты** содержит следующие блоки:

1. Название и логотип сервиса (header)
2. Ссылка на страницу публикации нового поста
3. Список опубликованных различными пользователями постов с фотографиями или видео (не менее трёх, хотя бы один с фото и один с видео). Каждый пост содержит:
	- имя пользователя, опубликовавшего пост;
	- одну фотографию ИЛИ одну видеозапись (последняя вставляется при помощи iframe, используйте youtube / vimeo / coub или любой другой видеохостинг);
	- текст пользователя, который может содержать хештеги. Хештегом называется слово или написанная слитно фраза, начинающаяся со знака # и идущая до ближайшего пробела (например #adukar #inlovewithworld #cherry2020 - три различных хештега). Каждый хештег в вёрстке оформляется как ссылка на страницу ленты с текстом хештега. Например ```<a href="feed.html">#adukar</a>```. Остальной текст никак не оформляется;
	- список комментариев к посту (может быть пустой), каждый комментарий содержит имя пользователя, оставившего комментарий, и текст комментария;
	- форму добавления комментария (должна включать только текстовое поле для ввода комментария).
	

**Страница создания нового поста** состоит из блоков:

1. Название и логотип сервиса (header)
1. Ссылка на страницу ленты
2. Форма создания нового поста, которая содержит следующие поля:
	- Текст поста, хештеги вводятся как обычный текст (необязательное поле)
	- Выбор файла фото или видео для загрузки (допустим выбор форматов jpg, png, mp4, для этого можно использовать [атрибут *accept*](https://developer.mozilla.org/ru/docs/Web/HTML/Element/Input/file#Limiting_accepted_file_types) тега *input*)

После отправки формы пользователя перенаправляет на страницу ленты.



## Задание 2. Форма заказа такси

### Техзадание

Сайт из трёх страниц (order-by.html, order-ru.html, order-en.html). Каждая страница написана на соответствующем языке и содержит:

1. Название и логотип проекта
2. Ссылки со страницами на других доступных языках
3. Форму заказа со следующими полями:
	- имя пользователя
	- адрес
	- телефон
	- тип оплаты (наличные / карта, реализовать с помощью радиокнопок)
	- тип автомобиля (базовый / премиальный / люкс, реализовать с помощью выпадающего списка)
	- дополнительные опции (минивэн / детское сидение / англоговорящий водитель, реализовать с помощью чекбоксов)
	- поле для комментариев
	- кнопка заказа
4. Контактную информацию сервиса заказа