## Модульное тестирование

**Цель работы:** изучить принципы и методы модульного (*unit*) тестирования, научиться разрабатывать, документировать и применять модульные тесты для проверки корректности работы программного кода.

**Задание:**
Реализовать программу согласно варианта на *Java* или *C#*. Написать *unit*-тесты, покрывающие все возможные варианты входных данных (некорректные и корректные данные). При некорректных входных данных генерировать свое собственное исключение (или использовать уже существующее, если оно полностью описывает характер ошибки). 

Учтите, что есть два основных вида исключений: проверяемые (необходимо обработать в `try/catch`) и непроверяемые (обрабатывать необязательно, можно генерировать при некорректных данных). Поэтому при реализации собственного класса-исключения Вы должны решить к какому типу он относится.

Использование библиотек, полностью решающих задачу, запрещено.  

Реализовать минимум 10 *unit*-тестов. Для некоторых вариантов в качестве эталона для теста можно использовать библиотеки, решающие задачу варианта. Для всех *unit*-тестов написать документацию - что тестируется, при каких условиях и ожидаемый результат.

**В отчете должно быть:**
- задание (первый абзац из этого документа)
- вариант реализуемой задачи
- краткое описание разработанной программы (список классов, методов)
- описание условий для корректной работы программы
- скриншоты с результатами работы программы и результатами прохождения тестов
- в приложении А: составить таблицу с тест-кейсами. Столбцы: 
	- идентификатор 
	- модуль программы (добавляем такой столбец, если тестируемых модулей несколько)
	- название тест-кейса и его описание (что тестируется, при каких условиях)
	- предварительные условия для выполнения теста (то, что должно быть выполнено перед выполнением теста)
	-  ожидаемый результат
- в приложении Б: текст программы
- в приложении В: текст модульных тестов

[Пример тест-кейса для unit-тестирования](https://github.com/the-hwk/GSTU-software-testing/blob/main/L4/%D0%9F%D1%80%D0%B8%D0%BC%D0%B5%D1%80%20%D1%82%D0%B5%D1%81%D1%82-%D0%BA%D0%B5%D0%B9%D1%81%D0%B0%20%D0%B4%D0%BB%D1%8F%20unit-%D1%82%D0%B5%D1%81%D1%82%D0%B8%D1%80%D0%BE%D0%B2%D0%B0%D0%BD%D0%B8%D1%8F.docx)

#### Варианты задач:

1. **Определение простого числа.** Вводится целое число, программа проверяет, является ли оно простым.
2. **Поиск наибольшего элемента в массиве.** Вводится список чисел, программа находит максимум.
3. **Нахождение НОД и НОК.** Вводятся два числа, программа вычисляет их НОД и НОК.
4. **Определение анаграммы.** Вводятся две строки, программа проверяет, являются ли они анаграммами.
5. **Сортировка массива пузырьком.** Вводится массив, программа сортирует его пузырьком.
6. **Разложение числа на простые множители.** Вводится число, программа выводит его разложение.
7. **Замена слов в строке.** Вводится строка и два слова, программа заменяет все вхождения одного слова на другое.
8. **Бинарный поиск в массиве.** Вводится массив и число, программа проверяет, есть ли число в массиве.
9. **Проверка палиндрома.** Вводится строка, программа проверяет, является ли она палиндромом.
10. **Шифр Цезаря.** Вводится строка и ключ, программа шифрует строку по алгоритму Цезаря.
11. **Перевод числа из десятичной системы в двоичную и обратно.**
12. **Решение квадратного уравнения.** Вводятся коэффициенты a, b, c, программа находит корни.
13. **Поиск самого длинного слова в строке.**
14. **Вычисление факториала.** Вводится число, программа вычисляет его факториал (учесть переполнение).
15. **Подсчет количества вхождений символа.** Вводится строка и символ, программа считает, сколько раз символ встречается.
16. **Генерация ряда Фибоначчи.** Вводится число N, программа генерирует N первых чисел ряда Фибоначчи.
17. **Форматирование телефонного номера.** Программа принимает ввод в произвольном формате и выводит его в виде `+7 (XXX) XXX-XX-XX`.
18. **Конвертация даты в текстовый формат.** Например: `12.03.2024 → 12 марта 2024 года`.
19. **Проверка числа на совершенность.** Определить, является ли число совершенным (равно сумме своих делителей, кроме самого себя).
20. **Удаление повторяющихся символов из строки.**
21. **Преобразование регистра текста.** Вводится строка, программа меняет регистр на противоположный.
22. **Калькулятор индекса массы тела:** Рассчитать индекс массы тела на основе роста и веса.
23. **Число Фибоначчи:** Определить `n`-е число Фибоначчи.
24. **Реверс строки:** Развернуть введенную строку.
25. **Подсчет гласных и согласных:** Подсчет количества гласных и согласных в строке.
26. **Конвертер валют:** Пользователь вводит сумму и валюту, программа переводит в другую валюту по курсу.
27. **Среднее арифметическое списка чисел:** Вычисляет среднее значение введенного списка чисел.
28. **Календарь дней месяца:** Принимает месяц и год, возвращает количество дней (учитывать год: високосный/невисокосный).
29. **Расчет стоимости поездки:** Пользователь вводит расстояние и расход топлива, программа считает затраты. Тесты: разные расстояния, отрицательные значения.
30. **Проверка IP-адреса:** Определяет, является ли введенная строка валидным IPv4-адресом.
