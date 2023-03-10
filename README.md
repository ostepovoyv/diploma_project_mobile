# Дипломный проект по тестирования мобильного приложения [Wikipedia](https://github.com/wikimedia/apps-android-wikipedia/)

<p align="center">
<img title="Wikipedia" name="Wikipedia" src="media/logo/Wikipedia.svg">
</p>

## :open_book: Содержание:

- [Технологии и инструменты](#technologist-технологии-и-инструменты)
- [Запуск тестов](#-запуск-тестов)
- [Запуск тестов в Jenkins](#-запуск-тестов-в-jenkins)
- [Отчет о результатах тестирования в Allure Report](#-отчет-о-результатах-тестирования-в-Allure-report)
- [Интеграция с Allure TestOps](#-интеграция-с-allure-testops)
- [Уведомления в Telegram](#-уведомления-в-telegram)
- [Пример запуска теста в Browserstack](#-пример-запуска-теста-в-Browserstack)

## :gear: Технологии и инструменты

<p align="left">
<a href="https://www.jetbrains.com/idea/"><img src="media/logo/Intelij_IDEA.svg" width="50" height="50"  alt="IDEA" title="IntelliJ IDEA"/></a>
<a href="https://www.java.com/"><img src="media/logo/Java.svg" width="50" height="50" alt="Java" title="Java"/></a>
<a href="https://gradle.org/"><img src="media/logo/Gradle.svg" width="50" height="50" alt="Gradle" title="Gradle"/></a>
<a href="https://junit.org/junit5/"><img src="media/logo/JUnit5.svg" width="50" height="50" alt="JUnit 5" title="JUnit 5"/></a>
<a href="https://github.com/"><img src="media/logo/GitHub.svg" width="50" height="50" alt="Github" title="GitHub"/></a>
<a href="https://developer.android.com/"><img src="media/logo/Android-studio.svg" width="50" height="50" alt="Android-studio" title="Android-studio"/></a>
<a href="https://appium.io/"><img src="media/logo/Appium.svg" width="50" height="50" alt="Appium" title="Appium"/></a>
<a href="https://www.browserstack.com/"><img src="media/logo/Browserstack.svg" width="50" height="50" alt="Browserstack" title="Browserstack"/></a>
<a href="https://github.com/allure-framework/allure2"><img src="media/logo/Allure_Report.svg" width="50" height="50" alt="Allure" title="Allure"/></a>
<a href="https://qameta.io/"><img src="media/logo/Allure_TO.svg" width="50" height="50" alt="Allure_TO" title="Allure_TO"></a>
<a href="https://www.jenkins.io/"><img src="media/logo/Jenkins.svg" width="50" height="50" alt="Jenkins" title="Jenkins"/></a>
<a href="https://web.telegram.org/"><img src="media/logo/Telegram.svg" width="50" height="50" alt="Telegram" title="Telegram"></a>
</p>

## :heavy_check_mark: Тест кейсы

- Поиск страницы BrowserStack
- Поиск страницы Microsoft, проверка на странице
- Прохождение онбординга
- Поиск по одной букве А
- Скрытие карточки на главной странице
- Проверка поиска (iOS)

# Запуск тестов
Для запуска тестов android:
```shell
gradle clean android -Denv=android
```

Для запуска тестов iOS:
```shell
gradle clean ios -Denv=ios   
```

Для локального запуска тестов:
```shell
gradle clean android -Denv=local  
```

## <img width="4%" title="Jenkins" src="media/logo/Jenkins.svg"> Запуск тестов в [Jenkins](https://jenkins.autotests.cloud/job/diploma_project_mobile/)

Сборка проекта.

<p align="center">
  <img src="media/screen/main_jenkins.png" alt="Jenkins" width="800">
</p>

## <img width="4%" title="Allure Report" src="media/logo/Allure_Report.svg"> Отчет о результатах тестирования в [Allure Report](https://jenkins.autotests.cloud/job/diploma_project_mobile/1/allure/)

<p align="center">
  <img src="media/screen/allure_1.png" alt="allure-report_1" width="900">
</p>

<p align="center">
  <img src="media/screen/allure_2.png" alt="allure-report_2" width="900">
</p>

## <img width="4%" title="Allure TestOPS" src="media/logo/Allure_TO.svg"> Интеграция с [Allure TestOps](https://allure.autotests.cloud/launch/19365/)

### Основной дашборд
<p align="center">
  <img src="media/screen/Allure_TO1.png" alt="Allure_TO1" width="900">
</p>

### Список тестов с результатами
<p align="center">
  <img src="media/screen/Allure_TO2.png" alt="Allure_TO2" width="900">
</p>

### Test plans
<p align="center">
  <img src="media/screen/Allure_TO3.png" alt="Allure_TO3" width="900">
</p>

## <img width="4%" title="Telegram" src="media/logo/Telegram.svg"> Уведомления в Telegram
После завершения сборки специальный бот, созданный в <code>Telegram</code>, автоматически обрабатывает и отправляет сообщение с отчетом о прохождении тестов.

<p align="center">
<img title="Telegram Notifications" src="media/screen/telegram_notify.png">

## <img width="4%" title="Browserstack" src="media/logo/Browserstack.svg"> Пример запуска теста в Browserstack

К каждому тесту в отчете прилагается видео.

<p align="center">
  <img title="Browserstack Video" src="media/video/mobile_test_video.gif">
</p>

[Вернуться к началу ⬆](#Wikipedia)