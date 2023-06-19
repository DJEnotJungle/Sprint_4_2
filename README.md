# Sprint_4

### Технологии в проекте:
**JUnit 4.13.2** - Для модульного тестирования  
**Selenium 3.141.59 и WebDriverManager 5.3.2** - Для выполнения задач автотестирования в браузере  
**Maven 3.9.0**  -  фреймворк для сборки проекта  
**Java 11**
### Предварительная настройка перед запуском тестов
Тест покрывает практически весь функционал описанных задач по умолчанию.   
Единственное что нужно выбрать перед первым запуском это количество суток аренды самоката во втором кейсе. Можно было конечно поместить перебор всех вариантов ввода в параметризированный тест, но  на мой взгляд это бы "переполнило" код и сделало бы его не очень удобным к прочтению.  
Поэтому перед запуском теста необходимо перейти в класс [RentScooter](src/main/java/ru/yandex/practicum/scooter/page/object/RentScooter.java) и выбрать необходимое значение локатора **`howManyTimeOfRent`**. По умолчанию выбрано значение 1 сутки.   
После настроек остаётся запустить необходимый тест.
### Описание классов
**[HomeFourPart](src/main/java/ru/yandex/practicum/scooter/page/object/HomeFourPart.java).** В этом классе описываются все необходимые методы и локаторы для автоматизации тестирования раздела FAQ.  
**[HomeFourPartTest](src/test/java/ru/yandex/practicum/scooter/page/object/HomeFourPartTest.java).** В этом классе как видно исходя из названия находится параметризированный автотест на проверку раздела FAQ.  
**[RentScooter](src/main/java/ru/yandex/practicum/scooter/page/object/RentScooter.java).** В этом классе описываются все необходимые методы и локаторы для автоматизации тестирования оформления заказа самоката.  
**[RentScooterTest ](src/test/java/ru/yandex/practicum/scooter/page/object/RentScooterTest.java).** В данном классе происходит происходит поверка оформления заказа с всевозможными комбинациями оформления заказа.