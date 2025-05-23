This section explains how to use basic operators in Python.

### Арифметични оператори

Както във всички други програмни езици, операторите за събиране, изваждане, умножение и деление могат да се използват с числа.<br>

    number = 1 + 2 * 3 / 4.0
    print(number)

Опитайте се да предвидите какъв ще бъде отговорът. Следва ли Python реда на операциите?

Друг наличен оператор е модулното (%) деление, което връща целочисления остатък от делението. divider % делител = остатък.

    remainder = 11 % 3
    print(remainder)

Използването на две символа за умножение създава връзка за повдигане на степен.

    squared = 7 ** 2
    cubed = 2 ** 3
    print(squared)
    print(cubed)

### Използване на оператори със стрингове

Python поддържа конкатениране на стрингове чрез оператора за събиране:

    helloworld = "hello" + " " + "world"
    print(helloworld)

Python също така поддържа умножаване на стрингове, за да се създаде стринг с повтаряща се последователност:

    lotsofhellos = "hello" * 10
    print(lotsofhellos)

### Използване на оператори със списъци

Списъците могат да бъдат обединени с оператора за събиране:

    even_numbers = [2,4,6,8]
    odd_numbers = [1,3,5,7]
    all_numbers = odd_numbers + even_numbers
    print(all_numbers)

Точно както и при стринговете, Python поддържа създаване на нови списъци с повтаряща се последователност с помощта на оператора за умножение:

    print([1,2,3] * 3)

Exercise
--------

Целта на това упражнение е да създадете два списъка, наречени `x_list` и `y_list`,
които съдържат 10 екземпляра на променливите `x` и `y`, съответно.
Също така трябва да създадете списък, наречен `big_list`, който съдържа
променливите `x` и `y`, по 10 пъти всяка, чрез конкатениране на двата създадени от вас списъка.