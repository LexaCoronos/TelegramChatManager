# ~ Telegram Bot «TelegramChatManager» ~

**Краткое описание:** Telegram бот-менеджер для контроля порядка в группе. Данный Telegram бот был написан на заказ для Telegram группы.

**Категория:** Разработка ботов.

**Ссылка:** Отсутствует. Бот не для публичного использования.

-----------------------------------

🔻 **Возможности:**

✅ Контроль флуда в группе, как от одного участника так и от многих.

✅ Возможность указать фразы для отправки ботом в чат в разных интервалах времени от простоя.

✅ Ответ бота по триггер фразам.

✅ Ночная статистика по количеству сообщений, картинок и топ болтунов за день.

✅ Контроль цензуры в чате.

✅ По хэштегу «#дайкартинку», бот формирует запрос и выдаёт изображение, которая больше не повторяется при повторном запросе. Изображение можно скачать в оригинальном качестве. У каждой картинки есть индивидуальный срок жизни 1 месяц.

✅ Возможность указать фразы для триггер времени.

✅ Бот логирует историю чата каждого пользователя и ведёт глобальный лог сообщений.

-----------------------------------

🔻 **Описание работы:**

-----------------------------------

🔹 Если 1 участник пишет более 5 сообщений подряд, бот отвечает ему "*Полегче, парнишка, мы не успеваем читать*".

Фразу можно менять в файле «**message.cfg**».

-----------------------------------

🔹 Если в чате тишина больше часа, бот присылает фразу из файла «**IntervalsAndPhrases.txt**» соответственно текущему часу.

И устанавливается задержка на 1 час, после чего бот начинает снова проверять этот пункт.

С **7:00** до **23:00** бот будет молчать.

Файл «**IntervalsAndPhrases.txt**» можно редактировать через текстовый редактор (лучше Notepad++),
устанавливая нужный интервал и соответствующую фразу к нему.

-----------------------------------

🔹 Если в чате проскакивает "*Слава Украине!*", бот отвечает "*Героям Слава!*".

-----------------------------------

🔹 Если в чате проскакивает слово «**поздравляю**» или «**вiтаю**», бот присылает «*О, присоединяюсь к поздравлениям!*», только 1 раз в день.

Фразу можно менять в файле «**message.cfg**».

-----------------------------------

🔹 Если в течение минуты появляется более 15 сообщений - бот выкидывает картинку кота с попкорном.

И устанавливается задержка на 1 минуту, после чего бот начинает снова проверять этот пункт.

-----------------------------------

🔹 В **00:02** бот выдает статистику по количеству сообщений, картинок, ссылок за день и выделяет 3 призовых места среди болтунов

-----------------------------------

🔹 Если в течение 5 минут проскакивает больше 10 матюков - бот присылает «*Что случилось? Предлагаю всем забухать!*».

И устанавливается задержка на 5 минут, после чего бот начинает снова проверять этот пункт.

Фразу можно менять в файле «**message.cfg**».

Фильтр плохих слов можно дополнять в файле «**BLACK_LIST_WORD.txt**».

Файл «**BLACK_LIST_WORD.txt**» можно редактировать через тектовый редактор (лучше Notepad++).

-----------------------------------

🔹 Бот умеет присылать картинки по запросу

«**#дайкартинку windows 10**».

Всё что написано после хэштега «**#дайкартинку**», будет формироваться в запрос и бот выдаёт одну картинку, которая больше не повторяется при повторном запросе.

По желанию картинку можно скачать в оригинальном качестве нажав на «**Скачать**» в описании картинки.

У каждой картинки есть индивидуальный срок жизни 1 месяц. После чего данная картинка будет очищаться из истории поиска и бот снова может её прислать.

-----------------------------------

🔹 Если кто-то отписывается с **04:00** до **06:00** утра, то бот отвечает – «*Ты охренел? Спать иди...писатель...*».

Фразу можно менять в файле «**message.cfg**».

-----------------------------------

❇️ Дополнительные возможности:

🔸 К тому же, в полночь бот удаляет историю чата из базы данных за все предыдущие дни (она попросту становится неактуальной).

🔸 Бот логирует историю чата каждого пользователя.
	
В папке **/logs/users** хранятся тектовые файлы логов под каждого пользователя -> "**username.txt**".
	
В папке **/logs** хранится глобальный лог всех обращений к боту -> "**global_user_log.txt**".

Файл **message.cfg**

![screen1](https://github.com/LexaCoronos/TelegramChatManager/blob/master/img/screenshot1.jpg)

Файл **IntervalsAndPhrases.txt**

![screen2](https://github.com/LexaCoronos/TelegramChatManager/blob/master/img/screenshot2.jpg)
