# Space Game Web

Space Game Web - это часть проекта вымышленной компании Tailspin, созданный Microsoft для обучения такому продукту, как Azure Devops.
Именно эта часть отвечает за отображение статистики прохождения игроками разных игр, созданных в Tailspin.

## С чего начать

Для использования данного проекта достаточно выполнить команду ```git clone https://gitlab.rebrainme.com/slozenkov_at_gmail_com/rebrain-devops-task1```.

### Необходимые требования

Необходимые инструменты, которые понадобятся для локальной работы с проектом, а также для его сборки и деплоя:
* Настроенная организация в Azure DevOps
* Установленный Visual Studio Code
* Установленный .NET Core 3.1
* Установленный Git
* Учетная запись в GitHub 

### Установка

Проект включает в себя несколько различных фреймворков и примерная последовательность получения рабочего приложения такова:

```
Запустить npm install для установки пакетов Node.js packages, определенных в package.json.
Запустить node-sass для преобразования Sass (.scss) файлов в CSS (.css) файлы.
Запустить gulp для минимизации файлов JavaScript and CSS.
Напечатать информации о текущем билде в каталог wwwroot directory, чтобы помочь команде QA идентифицировать билд по номеру и дате.
Запустить dotnet restore для установки всех зависимостей проекта.
Запустить dotnet build для сборки проекта в конфигурациях Debug и Release.
Запустить dotnet publish для упаковки приложения в .zip файл и копирования его, как результат, в сеиевую шару, где команда QA сможет забрать ее.
```

## Запуск тестов

Для запуска Unit-тестов необходимо выполнить команды:
```
dotnet build --configuration Release
dotnet test --configuration Release --no-build
```


### Дополнительные тесты

В репозитарии приложения также имеются следующие тесты:
* Code Coverage (Определение покрытия приложения unit-тестами)
* Vulnerabilities testing (Тестирование на уязвимости как самого кода, так и используемых библиотек)
* Functional testing (GUI тесты, использующие фреймворк Selenium)
* Load test (Нагрузочные тесты)

## Развертывание

Развертывание может быть осуществлено на платформе Microsoft Azure двумя путями:
* В виртуальную машину с Ubuntu
* В webapp

В обоих случаях, в репозитарии присутствует полный набор скриптов Terraform для создания необходимых объектов перед развертыванием.

## Собрано с использованием

* [.Net](https://dotnet.microsoft.com/) - The Microsoft developer platform
* [Node.js](https://nodejs.org/en/) - Javascript runtime

## Содействие

Продукт является собственностью компании Tailspin и возможность стороннего вмешательства в разработку польностью отсутствует.

## Versioning

Мы используем [SemVer](http://semver.org/) для версионирования. С имеющимися версиями можно ознакомиться на [теги в этом репозитории](https://gitlab.rebrainme.com/slozenkov_at_gmail_com/rebrain-devops-task1/-/tags). 

## Авторы

* **Andy** - *Основной разработчик* - [MainDragon](https://gitlab.rebrainme.com/slozenkov_at_gmail_com/)
* **Mara** - *Junior-разработчик* - [Tatsumi](https://gitlab.rebrainme.com/slozenkov_at_gmail_com/)

## Лицензирование

Проект использует, как открытые, так и закрытые лицензии. This project is licensed under the MIT License - see the [LICENSE.md](LICENSE.md) file for details


