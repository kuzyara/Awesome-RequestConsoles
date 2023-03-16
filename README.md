# Консоли запросов для 1С
Список всех популярных обработок

- Типовые
  - [Консоль запросов ИТС 8.1 | its.1c.ru](#консоль-запросов-итс-81--its1cru)
  - [Консоль запросов ИТС 8.2 | its.1c.ru](#консоль-запросов-итс-82--its1cru)
  - [Консоль запросов ИТС 8.3 | its.1c.ru](#консоль-запросов-итс-83--its1cru)
- Обычные формы
  - [Запросник 8.2 | makrus.ru | https://infostart.ru/public/72969/](#запросник-82--makrusru--httpsinfostartrupublic72969)
  - [Консоль запросов для обычных форм Павла Чистова | 1c.chistov.pro](#консоль-запросов-для-обычных-форм-павла-чистова--1cchistovpro)
- Обычные и управляемые формы
  - [Универсальная консоль запросов | programmist1s.ru](#универсальная-консоль-запросов--programmist1sru)
  - [Консоль запросов 1С | consquery.ru | https://infostart.ru/public/14183/](#консоль-запросов-1с--consqueryru--httpsinfostartrupublic14183)
  - [Консоль запросов с графом (Анализатор сложных запросов) | https://infostart.ru/public/617990/](#консоль-запросов-с-графом-анализатор-сложных-запросов--httpsinfostartrupublic617990)
- Управляемые формы
  - [Консолька | helpme1s.ru | https://infostart.ru/public/591653/](#консолька--helpme1sru--httpsinfostartrupublic591653)
  - [Консоль запросов для управляемого приложения 1С 8.2 - 8.3 | 1c-uroki.ru | https://infostart.ru/public/64522/](#консоль-запросов-для-управляемого-приложения-1с-82---83--1c-urokiru--httpsinfostartrupublic64522)
  - [Запросник 2.0 | itdemka.ru | https://infostart.ru/public/295356/](#запросник-20--itdemkaru--httpsinfostartrupublic295356)
  - [СДР: Консоль запросов Х (©ROL32) | https://infostart.ru/public/938606/](#сдр-консоль-запросов-х-rol32--httpsinfostartrupublic938606)
  - [Консоль запросов 9000 (©kuza2000) | github | https://infostart.ru/public/1190868/](#консоль-запросов-9000-kuza2000--github--httpsinfostartrupublic1190868)
  - [МегаКонсоль запросов 8.3 @AlexxSys | https://infostart.ru/public/331421/](#мегаконсоль-запросов-83-alexxsys--httpsinfostartrupublic331421)
  - [Консоль запросов для платформы 8.3.5 (©BigB) | kursypo1c.ru | https://infostart.ru/public/277749/](#консоль-запросов-для-платформы-835-bigb--kursypo1cru--httpsinfostartrupublic277749)
  - [Консоль запросов для платформы 1С 8.2-8.3 (©ТопчийДЮ) | https://infostart.ru/public/272459/](#консоль-запросов-для-платформы-1с-82-83-топчийдю--httpsinfostartrupublic272459)
  - [Управляемая консоль отчетов 3.8.9 (©Evg-Lylyk) | https://infostart.ru/public/835718/](#управляемая-консоль-отчетов-389-evg-lylyk--httpsinfostartrupublic835718)


# Типовые
  
## Консоль запросов ИТС 8.1 | [its.1c.ru](https://its.1c.ru/db/metod8dev#content:1645:hdoc)
https://its.1c.ru/db/files/1CITS/EXE/ExtReps/Unireps81/RequestConsole/RequestConsole.zip

Созданная в 2007 году, до сих пор популярна. Это [база ;)](https://www.youtube.com/watch?v=ejNGCWEgJNU)
- обычные формы

![image](https://user-images.githubusercontent.com/2604430/224766343-6b7a555c-2df2-4c3f-b0e1-8c0cd36af304.png)

## Консоль запросов ИТС 8.2 | [its.1c.ru](https://its.1c.ru/db/metod8dev/content/4500/hdoc)
https://its.1c.ru/db/files/1CITS/EXE/ExtReps/Unireps82/RequestConsoleManaged/RequestConsoleManaged.zip

Типовая консоль для УФ
- только управляемые формы
- поддерживает веб-клиент, тонкий клиент
- вывод плана выполнения запроса!
- текст запроса для конфигуратора, вывод данных временных таблиц, сравнение двух результатов запроса
- позволяет перенести запрос из отладчика (требуется БСП)

Примечание: если встречаете [ошибку](https://yadi.sk/i/qAu6m6b1ZNsfdg) "Ожидается выражение Выбрать" при вызове конструктора - вот [фикс](https://yadi.sk/i/wQyHwVxeYNYZ7w)

![image](https://user-images.githubusercontent.com/2604430/224768918-7f1a7171-8624-45ab-94f9-e1efd4a11376.png)

## Консоль запросов ИТС 8.3 | [its.1c.ru](https://its.1c.ru/db/metod8dev/content/4500/hdoc)
https://its.1c.ru/db/files/1CITS/EXE/ExtReps/Unireps83/RequestConsoleManaged/RequestConsoleManaged.zip

Является копией обработки 8.2, но:
- работает только для платформ 8.3.12+ ([использует](https://yadi.sk/i/6UkN8xDhWCgGDA) методы новой платформы)
- сохранение в файл плана запроса вместе с текстом запроса
- одновременная работа с файлом logcfg.xml из разных баз (разбивает конфиг на [блоки](https://yadi.sk/i/UpBLv7_6io0KTQ))
- получение планов запросов из параллельно открытых эксемпляров обработки в одном сеансе
- отключение ТЖ и удаление логов при закрытии обработки

![image](https://user-images.githubusercontent.com/2604430/224995700-d5ca98c3-3e8c-49e6-ac49-d076c911f693.png)

# Обычные формы

## Запросник 8.2 | [makrus.ru](https://makrus.ru/chastye-voprosy-po-1s/konsol-zaprosov-1s-dlja-obychnogo-prilozhenija-i-konsol-zaprosov-1s-dlja-upravljaemogo-prilozhenija.html) | https://infostart.ru/public/72969/
https://makrus.ru/files/files-1c/zaprosnik-8.2.rar

Компактная, но очень функциональная консоль, с необычным использованием панелей вместо модальных окон.
- обычные формы (в обработке всего одна форма!)
- храненит историю выполненных запроса
- формирование текста запроса для модуля
- установка момента времени, СЗ, ТЗ для параметров запроса
- Отладка запроса в модуле
- Выполнение алгоритма над результатом запроса

![image](https://user-images.githubusercontent.com/2604430/224739125-8a99bd0e-26ea-4f00-bc5f-98833c85e910.png)

## Консоль запросов для обычных форм Павла Чистова | [1c.chistov.pro](https://1c.chistov.pro/2009/06/blog-post.html)
https://romanpro.ru/files/1c/console.zip

Консоль отличается от стандартной с дисков ИТС следующими возможностями:
- Добавлен замер производительности (в заголовке окна)
- Возможность работы с пакетными запросами. Поддерживается метод ВЫПОЛНИТЬПАКЕТ
- Возможность отображения содержимого всех временных таблиц участвующих в запросе (бета)
- Возможность добавлять и удалять знаки переноса строки "|" в начале строк текста запроса (удобно для переноса текста из/в конфигуратор)
- Возможность получить полный текст запроса, от его описания до установки параметров нажатием на одну кнопку.
- Добавлено автосохранение настроек консоли между сеансами работы
- Добавлена опция работы только с выделенным текстом

![image](https://user-images.githubusercontent.com/2604430/225547841-e7c0d48f-a7a9-42fa-b62c-12193b869555.png)


## Консоль запросов 1С 8.2 УФ и ОФ | https://infostart.ru/public/177142/

Взята с http://infostart.ru/public/126781/. Доделал Санек ICQ 129193052. Несмотря на то что в публикации заявлено УФ, консоль управляемых форм лежит в архиве в виде отдельной обработки, которая была взята из другой публикации. Поэтому заводить её в категорию "УФ и ОФ" считаю неправильным. Пользуясь случаем, передаём Саньку привет)  Имеет 716+ скачиваний
- Консоль запросов оф и уф 8.3.5 (обычные формы в виде отдельной обработки, [скриншот](
- ))
- Только толстый клиент
- Вставка запроса из буфера обмена
- Консоль запросов для 1С 8.2 УФ

![image](https://user-images.githubusercontent.com/2604430/225598754-04a3e764-fa5d-447f-8edb-1eeadd02c16c.png)

# Обычные и управляемые формы

## Универсальная консоль запросов | [programmist1s.ru](https://programmist1s.ru/konsol-zaprosov-1s-opisanie-i-skachat/)
https://programmist1s.ru/wp-content/uploads/2013/05/KonsolZaprosovUniversalnaya_programmist1S.ru_-1.zip

Обработка с критичным багом в УФ, которая до сих пор держится в топе выдачи поисковиков. Похоже поддержка приостановлена в 2016 году.
- [обычные](https://user-images.githubusercontent.com/2604430/224759408-e1df0ea8-4163-458d-ad7f-2ac0cf5c1218.png) и управляемые формы
- обработка обычных форм взята с www.chistov.spb.ru
- перобразование текста запроса в код; позволяет просмотреть все промежуточные запросы в пакете запросов; позволяет увидеть результат, которые возвращают временные запросы в таблице
- предупреждение "Использование модальных окон запрещено" https://yadi.sk/i/wSjUXWXweTMtjw
- ошибка при открытии параметров https://yadi.sk/i/1Og4mBQyrrJ91Q
- ошибка "Открытие окон при завершении работы запрещено" https://yadi.sk/i/diqYFe0xxm4-jA
- нельзя использовать конструктор в тонком клиенте


![image](https://user-images.githubusercontent.com/2604430/224751773-3d9c36b9-a3f1-4689-a5e5-cebf41b4b8b3.png)

## Консоль запросов 1С | [consquery.ru](https://consquery.ru/) | https://infostart.ru/public/14183/
https://github.com/lavelinevgeny/consquery/raw/master/consquery83.epf

Консоль с богатым функционалом и болишим количеством вложенных в неё сил.
- [обычные](https://user-images.githubusercontent.com/2604430/224756077-cce6399a-889a-47d8-ad13-079b2538aaec.png) и управляемые формы!
- сохранение запросов в облако (не в gmail или yandex, а на сайт consquery.ru)
- выполнение запроса по списку ИБ
- множество действий с результатом запроса
- отладка запроса, выполнение кода 1С, автоподстановка (intellisence)
- предупреждение о режиме использования модальности при запуске в обычных формах https://yadi.sk/i/m1BzGwXxJawsEg
- заполнение параметров дублируется в обычных формах https://yadi.sk/i/aA1MsTp7uXB-RQ

![image](https://user-images.githubusercontent.com/2604430/224743811-da3eaf4b-f353-4fd6-b606-749f9853822f.png)

## Консоль запросов с графом (Анализатор сложных запросов) | https://infostart.ru/public/617990/

Консоль запросов для анализа запросов с большим количеством временных таблиц и вложенных запросов. Отображает структуру взаимосвязей временных таблиц в виде графа. Позволяет быстро передвигаться по тексту запроса и получать результат выполнения подзапросов.
- Поддержка УФ и [ОФ (скриншот)](https://yadi.sk/i/-eEGRp8en7KAYA)
- Плучение данных запроса из отладчика
- Текст запроса в структурированном виде (можно свернуть, развернуть текст подзапроса)

![image](https://user-images.githubusercontent.com/2604430/225593025-4a588d02-0ca3-4129-a5e4-4c5a6540551b.png)

# Управляемые формы
## Консолька | [helpme1s.ru](https://helpme1s.ru/obrabotka-konsol-zaprosov-sertakov-v-s-1s-8-2-8-3) | https://infostart.ru/public/591653/ (©Виталий Сертаков)
https://helpme1s.ru/files/sertakov/Query_Console_By_Sertakov.epf

Минималистичная консоль с необычным дизайном
- управляемые формы
- выполнения запроса к базам данных SQL!
- выполнения произвольного кода 1С

![image](https://user-images.githubusercontent.com/2604430/224772630-af4ee87d-106d-4495-941d-c44b8ec361cc.png)

## Консоль запросов для управляемого приложения 1С 8.2 - 8.3 | [1c-uroki.ru](http://1c-uroki.ru/articles/Konsol_zaprosov_1C_8.3_8.2) | https://infostart.ru/public/64522/ (©Николай Больсунов)

http://1c-uroki.ru/sites/default/files/articles/konsol_zaprosov_dlya_1s_8.3_i_8.2_0.zip

Простая удобная консоль без излишеств, 3518 скачиваний.
- управляемые формы
- конструктор работает только в толстом клиенте
- поддерживает вывод временных таблиц
- установка параметров типа момент времени и граница
- предупреждение "Использование модальных окон в данном режиме запрещено" https://yadi.sk/i/Kzi5qsCKCbzDkA
- модификация [обработки Больсунова](https://makrus.ru/files/files-1c/ConsSel_Managed_8_3.rar)

![image](https://user-images.githubusercontent.com/2604430/224735123-899244bc-90fb-4848-80cd-cd91cf81873c.png)

## Запросник 2.0 (©mrstomak) | [itdemka.ru](https://itdemka.ru/pubs/1122.html) | https://infostart.ru/public/295356/
https://itdemka.ru/11220.zip

Консоль на управляемых формах от автора, вдохновившегося запросником на обычных формах. 1700+ скачаваний.
- Возможность просмотра результата запроса в соответствии с настроенными выборками из него.
- Просмотр содержания временных таблиц результата запроса.
- Вызов консоли из текста программного модуля для отладки запроса.
- Замеры времени выполнения как запроса в целом, так и запросов пакета для создания временных таблиц.
- Отображение типов данных в результате запроса и отображение NULL. 
- Открытие на просмотр значений в результате запроса.
- Возможность выполнения произвольного программного алгоритма над результатом запроса.
- Есть модификация с загрузкой из табличного документа https://infostart.ru/public/608823/

![image](https://user-images.githubusercontent.com/2604430/225209748-894db27a-926e-456b-a1b8-273995cf120b.png)

## СДР: Консоль запросов Х (©ROL32) | https://infostart.ru/public/938606/
https://t.me/infostartfree/6490

Инструмент для программиста, позволяющий создавать и отлаживать запросы для баз 1С 8.3, а также обрабатывать результаты запросов (тонкий, толстый, web клиент). Не зависит от конкретной конфигурации, никаких БСП. 725+ скачиваний
- Работает с современными конфигурациями 1С (с запретом на использование модальности и синхронных вызовов)
- Заточена на интерфейс «Такси» - экономия места для работы по сравнению с неуправляемыми формами (можно погасить дерево запросов, результаты запроса)
- Оптимизирован обмен данными между клиентом и сервером
- Не содержит избыточного функционала, редко используемого в практической работе
- Для всех форм обработки установлен вариант масштаба "Компактный". 

![image](https://user-images.githubusercontent.com/2604430/225238740-9adcfa56-47a0-44df-8638-5ab97d85ca64.png)

## Консоль запросов 9000 (©kuza2000) | [github](https://github.com/hal9000cc/RequestConsole9000) | https://infostart.ru/public/1190868/
https://github.com/hal9000cc/RequestConsole9000/blob/master/releases/1.1.10/КонсольЗапросов9000.epf

Консоль мечты! По крайней мере так утверждает автор.) Работает на любой конфигурации без ее модификации. 654+ скачиваний
- полноценная работа в режиме управляемых форм в режиме толстого и тонкого клиента
- поддержка всех типов 1С, в том числе момента времени, границы, уникального идентификатора, типа «Тип», вида движений, таблиц значений (табличные части), и т.д.
- отладка запросов, перехват любых запросов из отладчика вместе с параметрами и временными таблицами
- работает при запрете синхронных методов
- сохранение комментариев в запросах после конструктора
- вставка предопределенных значений
- передача результата запроса в параметрах
- обработка результата запроса кодом
- получение текста запроса СУБД, плана запроса, отображение текста и плана запроса в терминах 1С
- возможность работы в составе расширения

![image](https://user-images.githubusercontent.com/2604430/225509688-6bbeb4d3-2582-4c1a-8176-fcaa61b8f89d.png)

## МегаКонсоль запросов 8.3 @AlexxSys | https://infostart.ru/public/331421/
https://mega.nz/file/2YFiAb4C#GHfmAGEqfAhiPVFGrSHgwvDzeroRtBEOOTDrQstyjOM

Более продвинутая версия консоли запросов, как по функциям, так и по интерфейсу. Имеет полностью переработанный интерфейс, с более понятным расположением панелей кнопок. Также добавлен нужный функционал - структура конфигурации, с возможностью добавления в запрос таблиц и полей и справка по синтаксису запросов. 574+ скачиваний
- Встроен механизм, формирующий структуру конфигурации, со всеми виртуальными таблицами (СрезПоследних, Остатки, Обороты и т.д.) . При выборе любого объекта или реквизита, его путь переносится в текст запроса.
- Встроена справка по синтаксису и основным конструкциям запроса. Так как при написании любых сложных запросов, или их редактировании, оптимизации лучше пользоваться ручками, а не конструктором, то справочник по всем функциям помогает в этом деле.
- Реализован выбор типа в параметрах, разделенный в дереве на типы методанных (Примитивные, Справочники, Документы, Бизнесс-процессы ...)
- Переделан интерфейс, все кнопки разделены по своим сферам влияния

![image](https://user-images.githubusercontent.com/2604430/225534928-fd143c11-f160-479d-9acc-c92296a1e391.png)

## Консоль запросов для платформы 8.3.5 (©BigB) | [kursypo1c.ru](https://курсы-по-1с.рф/articles/1с-предприятие-8-3-5-конструктор-запросов/) | https://infostart.ru/public/277749/
https://fs.kursypo1c.ru/free/КонсольЗапросов_8.3.5.epf

Когда вышла новая платформа 8.3.5, в ней сделали возможность запускать консоль запросов не только в толстом клиенте, но и тонком и веб клиенте. 649+ скачиваний
- за основу взята консоль запросов для управляемого приложения с диска ИТС
- работает в тонком и веб клиенте.

![image](https://user-images.githubusercontent.com/2604430/225536708-ac11090b-1e42-41c4-a3fe-bef7bd20e8a4.png)

## Консоль запросов для платформы 1С 8.2-8.3 (©ТопчийДЮ) | https://infostart.ru/public/272459/

Данная консоль запросов является доработанной версией стандартной консоли с сайта ИТС т.к. нужного и удобного функционала не было найдено. Для модернизации были взяты наработки из консоли http://infostart.ru/public/126781/ 403+ скачиваний
- Управляемое приложение, Такси
- конструктор работает ТОЛЬКО в толстом клиенте
- были устранены выявленные ошибки в обеих обработках

![image](https://user-images.githubusercontent.com/2604430/225538899-1ffb1154-d180-4e69-8ffb-0d3a1ca4f15a.png)

## Управляемая консоль отчетов 3.8.9 (©Evg-Lylyk) | https://infostart.ru/public/835718/

Консоль на управляемых формах с самыми разнообразными возможностями. Поддержка бесплатной версии прекращена, так как разработка перешла в разряд коммерческих [Консоль разработчика (IS Toolkit)](https://infostart.ru/public/1254364/). 1393+ скачиваний
- Работа с запросом и СКД, Полная поддержка пакетных запросов, временных таблиц, Сравнение результатов, текстов, Разбор структуры запроса в виде дерева,
- Анализ плана запроса, Групповая обработка.
- Поддержка английского языка!
- Реализован отказ от модальности и синхронных вызовов
- режим совместимости 8.3.10+
- имеет свой youtube канал
- имеет подробный сравнительный (список фич)[https://cloud.mail.ru/public/8ACQ/hm7waFRp6]

![image](https://user-images.githubusercontent.com/2604430/225584380-a4eb7d5d-cf88-4665-8ea0-9f3c51d44857.png)

## Консоль запросов, версия 1.8.1 | https://infostart.ru/public/126781/

Консоль запросов 1.8.1 разработана для использования в тонком и толстом клиенте управляемого приложения. 1229+ скачиваний
- Работает начиная с версии платформы 8.3.3
- Интеграция с режимом отладки
- конструктор запросов доступен только в режиме толстого клиента

![image](https://user-images.githubusercontent.com/2604430/225602991-5777345c-0d2c-4e4e-b348-d72ef89b89b6.png)

todo

* https://infostart.ru/public/331421/ (done) Консоль запросов 8.3 @AlexxSys
* https://infostart.ru/public/277749/ (done) Консоль запросов для платформы 8.3.5
* https://infostart.ru/public/295356/ (done) Запросник 2.0 на управляемых формах
* https://infostart.ru/public/1492536/ Совместимая консоль запросов для платформы 8.2 и 8.3 (низкое качество, 16 скачиваний)
* https://infostart.ru/public/272459/ (done) Консоль запросов для платформы 1С 8.2-8.3 (Управляемое приложение, Такси) 403 скачивания
* https://infostart.ru/public/64522/ (done) Консоль запросов для управляемого приложения 1С 8.2 - 8.3 (Такси) 3518 скачиваний
* https://1c.chistov.pro/2009/06/blog-post.html (done) 
* http://devtool1c.ucoz.ru/
* https://infostart.ru/public/126781/ Консоль запросов, версия 1.8.1 для управляемого приложения тонкий клиент. Интеграция с режимом отладки 1300 скачиваний
* https://infostart.ru/public/177142/ Консоль запросов 1С 8.2 УФ и ОФ 716	скачиваний
* https://infostart.ru/public/835718/ (done) Управляемая консоль запросов, отчетов 3.8.9 (расширение, внешняя обработка) 1392 скачиваний
* https://infostart.ru/public/938606/ (done) Консоль запросов для управляемых форм 8.3 СДР! (@ROL32), 725 скачиваний
* https://github.com/hal9000cc/RequestConsole9000 (done) Консоль запросов 9000
* https://infostart.ru/public/617990/ (done) Консоль запросов с графом (Анализатор сложных запросов)


