# Автоматизируемые сценарии:
1.	Позитивный сценарий покупки с APPROVED дебетовой карты. Используется номер APPROVED карты, зашитый в json, покупка проходит.
2.  Позитивный сценарий покупки тура в кредит с APPROVED дебетовой карты. Используется номер APPROVED карты, зашитый в json, покупка проходит.
3.  Негативный сценарий покупки с DECLINED дебетовой карты. Используется номер DECLINED карты, зашитый в json, покупка не проходит.
4.  Негативный сценарий покупки в кредит через DECLINED карту. Используется номер DECLINED карты, зашитый в json, покупка не проходит.
5.  Негативный сценарий покупки с несуществующей карты. Данные карты генерируются при помощи Faker. Покупка должна быть отклонена.
6.  Негативный сценарий покупки в кредит с несуществующей карты. Данные карты генерируются при помощи Faker. Покупка должна быть отклонена.
7.  Негативный сценарий  - отправка формы с пустыми полями при покупке с карты. Покупка должна быть отклонена.
8.  Негативный сценарий - отправка формы с пустыми полями при покупке в кредит. Покупка должна быть отклонена.

# Инструменты
1.  Gradle  - система сборки, удобная для прогона автотестов.
2.	JUnit – широко используемый фреймворк для автотестов
3.	Faker – позволит автоматически создавать данные для тестов
4.	Selenide – удобный экономичный фреймворк для UI тестов
5.	Docker – позволяет запускать контейнер с SQL
6.	Allure – простая понятная система репортинга
7.  MySQL и PostgreSQL согласно заданию
8.  DBeaver для просмотра баз данных


# Перечень и описание возможных рисков при автоматизации
1. Времени на автоматизацию тестирования уйдет больше, чем если бы провели ручное тестирование
2. "В реальной жизни приложение не должно пропускать через себя данные карт, если у него нет PCI DSS, но мы сделали именно так" - мы тестируем приближенный вариант сервиса, а не сам сервис как он будет работать, соответственно есть вероятность что при тестировании на проде мы получим ошибку там, где на моке у нас все тесты были зелёные.


# Интервальная оценка с учётом рисков в часах
1. Прохождение тестового сценария вручную и написание бег-репортов - 3 часа
2. Настройка тестового окружения - 8 часов
3. Написание дата-классов - 4 часа
4. Настройка SQL - 6 часов
5. Написание Page Objects - 8 часов
6. Написание позитивного теста - 3 часа
7. Написание негативных кейсов - 6 часов
8. Настройка репортинга - 1 час
9. Подготовка отчётов по тестированию - 4 часа.

*Итого*  43 часа

# План сдачи работ

1. 26 апреля 2023 - сдача плана тестирования
2. 27-30 апреля - написание автотестов и подготовка тестового окружения
3. 1 мая - подготовка отчетности по автотестам
4. 2 мая - подготовка отчетности по автоматизации