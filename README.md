# goit-js-hw-02

Задача 2-1

Использование for Напиши функцию getItemsString(array), которая получает массив
и возвращает строку, полученную из объединения (конкатенации) строк в формате
${номер элемента} - ${значение элемента}\n , где \n - спецсимвол переноса.

Нумерация должна начинаться с 1. К примеру для первого элемента массива
['Mango', 'Poly', 'Ajax'] с индексом 0 будет выведено '1 - Mango', а для индекса
2 выведет '3 - Ajax'.

Используйте вспомогательную переменную result для добавления (конкатенации)
строк внутри цикла for ///////////////////////////////////

Задача 2-2

Подсчет стоимости гравировки украшений Напиши скрипт подсчета стоимости
гравировки украшений. Для этого создай функцию calculateEngravingPrice(message =
"", pricePerWord = 0) принимающую строку (в строке будут только слова и пробелы)
и цену гравировки одного слова, и возвращающую цену гравировки всех слов в
строке.

Для решения этой задачи не используйте циклы. Т.е. никаких for, while, do while,
for of, for in, forEach или функциональных методов.////

/////// Задача 2-3

Поиск самого длинного слово в строке с пробелами Напиши функцию
findLongestWord(string = ""), которая принимает параметром произвольную строку
(в строке будут только слова и пробелы) и возвращает самое длинное слово в этой
строке.////

////// Задача 2-4

Форматирование строки в зависимости от длинны строки Напиши функцию
formatString(string, maxLength = 40) которая принимает строку и форматирует ее
если необходимо.

Если длина строки не превышает maxLength, функция возвращает ее в исходном виде.
Если длина больше maxLength, то функция обрезает строку до размера maxLength
символов и добавляет в конец строки троеточие ..., после чего возвращает
укороченную версию.///

////Задача 2-5 ///

Функция предикат Функция предикат возвращает true или false

Напиши функцию checkForSpam(message), принимающую 1 параметр message - строку.
Функция проверяет ее на содержание слов spam и sale. Если нашли запрещенное
слово то функция возвращает true, если запрещенных слов нет функция возвращает
false. Слова в строке могут быть в произвольном регистре.//// /// //Задача
2-6/// Конструкция new Array(10) создаст массив, длинной в 10 элементов.
Значения в таком массиве будут отсутствовать, т.е. не будет даже undefined.
Поэтому такой массив нужно заполнить значениями для дальнейшего использования.

Есть еще способ создания и заполнения массива - можно создать пустой массив [] и
заполнять его методом push()

Быстрая обработка массива Преимущество создания массива заданной длины перед
добавлением в пустой массив в том, что метод push() медленнее обрабатывается.

Если `new Array()` будет содержать более одного аргумента, то будет создан
массив с элементами из аргументов. Пример:

new Array(3); // [,,]

new Array(1, 2, 3); // [1, 2, 3] Быстрое создание массива Пустой массив. Вызов
new Array() создаст пустой массив []. Но это более медленный способ создания
массива по сравнению с использованием литерала. Если нужен пустой массив, то
рекомендуется использовать литерал массива.

const arrFast = []; // быстрее const arrSlow = new Array(); // медленнее
Создание нового массива на основе преобразования данных из старого массива
Напиши функцию mapArray(array), принимающую 1 параметр array - массив чисел.
Функция создает новый массив numbers размером в длину массива array и заполняет
его числами из массива array умноженными на 10. Для перебора массива и
добавления новых значений используй цикл for. По завершению перебора массива
array возвращается массив numbers. ///

///Задача 2-7///

Создание нового массива на основе отбора из исходного массива Напиши функцию
filterArray(array), принимающую 1 параметр array - массив. Функция проверяет
каждое значение массива - является ли значение конечным числом
(Number.isFinite). Для проверки используй цикл for. Числа добавляются в новый
массив numbers с помощью метода push, а не числа - игнорируются. По завершению
проверки массива array возвращается массив numbers./// ///

/// ///Задача 2-8//

/// Вычисление суммы массива Напиши функцию reduceArray(array), которая
принимает числовой массив array. Если массив array не пустой, необходимо
посчитать сумму всех элементов массива, используя цикл for. Для подсчета суммы
используй переменную total. Функция должна возвращать 0 если массив пустой и
значение total в противном случае.//

/// Задача 2-9////

Есть массив logins с логинами пользователей. Напиши скрипт добавления логина в
массив logins. Добавляемый логин должен:

проходить проверку на длину от 4 до 16-ти символов включительно быть уникален,
то есть отсутствовать в массиве logins Разбей задачу на подзадачи с помощью
функций. Проверку на отсутствие аргументов или на правильный тип аргументов
делать не нужно.

Напиши функцию isLoginValid(login), в которой проверь количество символов
параметра login и верни true или false в зависимости от того, попадает ли длина
параметра в заданный диапазон от 4-х до 16-ти символов включительно.

Напиши функцию isLoginUnique(allLogins, login), которая принимает список всех
логинов и добавляемый логин как параметры и проверяет наличие login в массиве
allLogins, возвращая true если такого логина еще нет и false если логин уже
используется.

Напиши функцию addLogin(allLogins, login) которая:

Принимает новый логин и массив всех логинов как параметры Проверяет валидность
логина используя вспомогательную функцию isLoginValid Если логин не валиден,
прекратить исполнение функции addLogin и вернуть строку 'Ошибка! Логин должен
быть от 4 до 16 символов' Если логин валиден, функция addLogin проверяет
уникальность логина с помощью функции isLoginUnique Если isLoginUnique вернет
false, тогда addLogin не добавляет логин в массив и возвращает строку 'Такой
логин уже используется!' Если isLoginUnique вернет true, addLogin добавляет
новый логин в logins и возвращает строку 'Логин успешно добавлен!' 🔔 Принцип
единственной ответственности функции - каждая функция делает что-то одно. Это
позволяет переиспользовать код и изменять логику работы функции только в одном
месте, не затрагивая работу программы в целом.

Предикатные функции возвращают только true или false. Такие функции принято
называть начиная с is: isLoginUnique и isLoginValid в нашем случае.

isLoginUnique только проверяет есть ли такой логин в массиве и возвращает true
или false. isLoginValid только проверяет валидный ли логин и возвращает true или
false. addLogin добавляет или не добавляет логин в массив. При этом для проверок
условия добавления использует результаты вызовов других функций - isLoginUnique
и isLoginValid.
