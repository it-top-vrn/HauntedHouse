[![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://github.com/itstep-vrn/HauntedHouse/blob/master/LICENSE) [![CodeFactor](https://www.codefactor.io/repository/github/itstep-vrn/hauntedhouse/badge)](https://www.codefactor.io/repository/github/itstep-vrn/hauntedhouse) [![Gitter](https://badges.gitter.im/itstep-vrn/HauntedHouse.svg)](https://gitter.im/itstep-vrn/HauntedHouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)

# Haunted House

Консольная игра с загадками

___
* **Игра, в которой нужно выбраться из дома с привидением**
* **© Маслякова Диана, 2019**
* **© Компьютерная академия ШАГ. Воронеж, 2019**
* **Версия: 0.1 (Июль 2019)**
___

## Описание игры

Нужно выбраться из подвала дома с привидением. 

Каждая дверь открывается путем отгадывания загадки, написанной на двери.

Ответом на каждую загадку будет число, которое нужно ввести. Есть три попытки около каждой двери.

Если число введено верно, то игрок проходит дальше. И в конце концов выйдет из дома.

Если число введено неверно, то на игрока нападает привидение и он остается в доме.

#### Реализация вариантов игры

Проигрыш

![Alt Text](https://github.com/itstep-vrn/HauntedHouse/blob/master/Loss.gif)


Выигрыш

![Alt Text](https://github.com/itstep-vrn/HauntedHouse/blob/master/Win.gif)


## Воспроизведение

* Консоль
* Ответы необходимо вводить ЦИФРАМИ

## Начало работы

Скопируйте файл .exe в любое место на вашем компьютере. Если у вас установлена программа Visual Studio, игра запустится.  
Если программа Visual Studio не установлена, система может запросить следующие файлы: msvcp140d.dll, vcruntime140.dll, ucrtbased.dll —  это компоненты пакета от корпорации Microsoft Visual C++ 2015.  
Скачайте данные файлы и разместите в корневой директории windows:  
- `C:\Windows\System32` для x32 системы;
- `C:\Windows\SysWOW64` для x64 системы.  
Перезагрузите компьютер и запустите программу.

***Скачать файлы для Windows 10 и других версий можно пройдя по ссылкам:***  

Для x64:  

- [msvcp140d.dll](http://dlltop.ru//files/msvcp140d-64.zip)  
- [vcruntime140.dll](http://dlltop.ru//files/vcruntime140-64.zip)  
- [ucrtbased.dll](http://dlltop.ru//files/ucrtbase-64.zip )  

Для x32: 

- [msvcp140d.dll](http://dlltop.ru//files/msvcp140d.zip)  
- [vcruntime140.dll](http://dlltop.ru//files/vcruntime140.zip)  
- [ucrtbased.dll](http://dlltop.ru//files/ucrtbase.zip)


## Описание кода программы:

### Подключение библиотек и пространства имен:
```cpp
    #include<iostream> //Библиотека ввода и вывода информации
    using namespace std //Использование стандартного пространства имен
```
    
### Основные функции:

- `void FirstDoor()` - Открытие первой двери
- `void SecondDoor()` - Открытие второй двери
- `void ThirdDoor()` - Открытие третьей двери
- `void TheEnd()` - Вывод выигрышного финала
- `void TheLoss()` - Проигрыш
