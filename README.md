Базовый каркас Symfony 2 для Ailove Factory
========================

Этот документ содержит информацию о том, как загрузить и начать использовать Symfony 2 в окружении Ailove Factory.

1) Загрузка
--------------------------------

Если вы уже скачали каркас приложения и распаковали/переместили его в корневой каталог виртуального хоста веб-сервера, пропустите этот шаг и перейдите к разделу "Установка".

Чтобы загрузить базовый каркас Symfony 2 для Ailove Factory, у вас есть два варианта:

### Скачать архив

Самый простой способ - скачать ZIP архив данного репозитория и распаковать его в соответсвующую директорию виртуального хоста веб-сервера.

### Клонировать репозиторий

Выполните в консоли следующие команды:

    cd path_to_dir
    git clone https://github.com/ailove-dev/sf2-base.git ./
    rm -rf .git

2) Установка
---------------

### a) Проверьте параметры системы (окружения)

Прежде чем начать, убедитесь, что ваша локальная система настроена правильно
для Symfony. Для этого выполните следующее:

    php app/check.php

Если вы получаете предупреждения или рекомендации, исправьте их перед тем как продолжить.

### b) Установите библиотеки вендоров

    php bin/vendors install

Примечание: у вас **должен** быть установлен **git**, т.к. при установке будут выполняться `git` команды.

### c) Доступ к приложению из браузера

Проверить состояние приложения можно по ссылке:

    http://virtual_host.lo/config.php

Если все хорошо, перейдите по ссылке "Bypass configuration and go to the Welcome page", чтобы загрузить первую страницу Symfony.


Вы так же можете увидеть реальный пример рабочей страницы:

    http://virtual_host.lo/app_dev.php

3) Запуск базового теста

    php app/console --env=test behat

4) Узнать больше о Symfony!
-----------------------

Отличный способ начать обучение Symfony прочитать краткий обзор [Quick Tour](http://symfony.com/doc/current/quick_tour/the_big_picture.html) который познакомит вас с основными возможностями Symfony 2.

После этого вы можете перейти к чтению официальной документации фреймворка [Symfony2 Book](http://symfony.com/doc/current/).

Bundles:
---------------
Данный каркас включает следующие пакеты (bundles):

* **FrameworkBundle**
* **SensioFrameworkExtraBundle** ([documentation](http://symfony.com/doc/current/bundles/SensioFrameworkExtraBundle/index.html))
* **DoctrineBundle** ([documentation](http://symfony.com/doc/current/book/doctrine.html))
* **TwigBundle** ([documentation](http://symfony.com/doc/current/book/templating.html))
* **SecurityBundle** ([documentation](http://symfony.com/doc/current/book/security.html))
* **SwiftmailerBundle** ([documentation](http://symfony.com/doc/2.0/cookbook/email.html))
* **MonologBundle** ([documentation](http://symfony.com/doc/2.0/cookbook/logging/monolog.html))
* **AsseticBundle** ([documentation](http://symfony.com/doc/2.0/cookbook/assetic/asset_management.html))
* **JMSSecurityExtraBundle** ([documentation](http://symfony.com/doc/current/bundles/JMSSecurityExtraBundle/index.html))
* **WebProfilerBundle**
* **SensioDistributionBundle**
* **SensioGeneratorBundle** ([documentation](http://symfony.com/doc/current/bundles/SensioGeneratorBundle/index.html))
* **buzz**
* **SahiClient**
* **MinkBundle**
* **Mink**
* **BehatBundle**
* **Gherkin**
* **Behat**
* **HelloBundle**
