# Отчёт о тестировании приложения KeyValidator

## Краткое описание

07.05.2021 было проведено тестирование приложения KeyValidator положительными и отрицательными данными.

На тестирование затрачено: 2 часа

В результате тестирования выявлены следующие дефекты: [Issue #1](https://github.com/goso-nct/netology-java-dz1.1-t2/issues/1)

Инструкцию по установке OpenJDK11 не проверял - там на картинках старая версия.
Приложение запускается и совместимо с Java 11.
Приложение работает согласно руководству использования.

## Описание процесса тестирования

В качестве тестовых использовались данные из [Руководства использования](https://github.com/netology-code/javaqa-homeworks/blob/master/intro/user-manual.md)

Были созданы два bat файла для запуска тестируемого класса с положительными (validate-ok.bat) и отрицательными (validate-fail.bat) данными.

### Положительное тестирование:

8f05e6a7-70e9-33d7-bfe7-b19eae0d8998  Ex.R: OK,  Act.R: OK  
80b427f8-92cd-3aae-ba04-03927fbe17c6  Ex.R: OK,  Act.R: **FAIL**  
b295bc63-9f03-3b4b-af80-969b39f8c262  Ex.R: OK,  Act.R: OK  
387eedc6-12e9-3b32-9881-63b6b5e85317  Ex.R: OK,  Act.R: **FAIL**  
c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180  Ex.R: OK,  Act.R: OK  

### Отрицательное тестирование:

18252235-78e0-44a5-8720-556f0c7da17a  Ex.R: FAIL, Act.R: FAIL  
e66075b6-ddad-445e-baf6-161b3289522b  Ex.R: FAIL, Act.R: FAIL  
b6d53250-f07e-4352-a293-6102ddf7f1ca   Ex.R: FAIL, Act.R: FAIL  
c2bc778a-1cb9-46c6-b435-0489649d2a42   Ex.R: FAIL, Act.R: FAIL  
2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1   Ex.R: FAIL, Act.R: **OK**  

## Тестирование производилось в следующем окружении:
* Windows 10 Pro 20H2 64bit
* AdoptOpenJDK-11.0.11+9 64bit HotSpot
