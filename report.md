# Отчёт о тестировании приложения KeyValidator

## Краткое описание

07.05.2021 было проведено тестирование приложения KeyValidator положительными и отрицательными данными.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты:  
* [Приложение валидирует неправильный ключ](https://github.com/goso-nct/netology-java-dz1.1-t2/issues/5)  
* [Приложение не валидирует правильный ключ](https://github.com/goso-nct/netology-java-dz1.1-t2/issues/6)


Установка OpenJDK11 по [инструкции](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/openjdk11-manual.md) прошла успешно (*не проверял*).  
Приложение запускается и совместимо с Java 11.  
Приложение работает согласно руководству использования.  

## Описание процесса тестирования
В рабочую папку был загружен класс из [ДЗ 1.1.2](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/artifacts/KeyValidator.class)  
Там же были созданы два bat файла для запуска тестируемого класса с положительными (validate-ok.bat) и отрицательными (validate-fail.bat) данными.  
В качестве тестовых использовались данные из [Руководства использования](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)  
Тестирование осуществлялось выполнением bat-файлов.

Полученные результаты:

**Положительное тестирование (выполнение validate-ok.bat):**

Result for 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998: OK  
Result for 80b427f8-92cd-3aae-ba04-03927fbe17c6: FAIL  
Result for b295bc63-9f03-3b4b-af80-969b39f8c262: OK  
Result for 387eedc6-12e9-3b32-9881-63b6b5e85317: FAIL  
Result for c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180: OK  

**Отрицательное тестирование (выполнение validate-fail.bat):**

Result for 18252235-78e0-44a5-8720-556f0c7da17a: FAIL  
Result for e66075b6-ddad-445e-baf6-161b3289522b: FAIL  
Result for b6d53250-f07e-4352-a293-6102ddf7f1ca: FAIL  
Result for c2bc778a-1cb9-46c6-b435-0489649d2a42: FAIL  
Result for 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1: OK  

## Тестирование производилось в следующем окружении:
* Windows 10 Pro 20H2 64bit
* AdoptOpenJDK-11.0.11+9 64bit HotSpot
