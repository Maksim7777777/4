# Автоматизируемые сценарии:
1.	Позитивный сценарий покупки с APPROVED дебетовой карты, покупка проходит. Номер карты APPROVED -4444 4444 4444 4441.
2.  Позитивный сценарий покупки тура в кредит с APPROVED дебетовой карты, покупка проходит. Номер карты APPROVED -4444 4444 4444 4441.
3.  Негативный сценарий покупки с DECLINED дебетовой карты, покупка не проходит. Номер DECLINED 4444 4444 4444 4442.
4.  Негативный сценарий покупки в кредит через DECLINED карту, покупка не проходит. Номер DECLINED 4444 4444 4444 4442
5.  Негативный сценарий покупки с несуществующей карты. Данные карты генерируются при помощи Faker. Покупка должна быть отклонена.
6.  Негативный сценарий покупки в кредит с несуществующей карты. Данные карты генерируются при помощи Faker. Покупка должна быть отклонена.
7.  Негативный сценарий  - отправка формы с пустыми полями при покупке с карты. Покупка должна быть отклонена.
8.  Негативный сценарий - отправка формы с пустыми полями при покупке в кредит. Покупка должна быть отклонена.

# Инструменты
1.  Gradle  - система сборки для прогона автотестов.
2.	JUnit – фреймворк для автотестов
3.	Faker – позволит автоматически создавать данные для тестов
4.	Selenide – фреймворк для UI тестов
5.	Docker – позволяет запускать контейнер с SQL
6.	Allure – система репортинга
7.  MySQL и PostgreSQL согласно заданию
8.  DBeaver для просмотра баз данных


# Перечень и описание возможных рисков при автоматизации
1. Времени на автоматизацию тестирования уйдет больше, чем если бы провели ручное тестирование



# Интервальная оценка с учётом рисков в часах
1. Настройка тестового окружения - 8 часов
2. Написание дата-классов - 5 часа
3. Настройка SQL - 7 часов
4. Написание Page Objects - 8 часов
5. Написание позитивного теста - 4 часа
6. Написание негативных кейсов - 7 часов
7. Настройка репортинга - 1 час
8. Подготовка отчётов по тестированию - 4 часа.

*Итого*  44 часа

# План сдачи работ

1. 15 мая 2023 - сдача плана тестирования
2. 17-23 мая - написание автотестов и подготовка тестового окружения
3. 25 мая - подготовка отчетности по автотестам
4. 27 мая - подготовка отчетности по автоматизации
