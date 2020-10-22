# Lab 2a
## Хід роботи
1. Створив файл trial.py. В даному файлі буду виконувати наступні підпункти. <br/>
    * Вивів на екран константи мови Python
        ##### Код програми:
            print("First constant", False)
            print("Second constant", True)
            print("Third constant", None)
        ##### Результат виконання:
            user@Pc:~/Python$ python3 trial.py
            First constant False
            Second constant True
            Third constant None
    * Вивів на екран результат виконання вбудованих функцій <br/> (Взяв функції, що починаються з букви мого прізвища)
        ##### Код програми:
            print("1", f"in bool function is {bool(1)}")
            print("0", f"in bool function is {bool(0)}")
            print("Number 21", f"in binary is {bin(21)}")
        ##### Результат виконання:
            user@Pc:~/Python$ python3 trial.py 
            1 in bool function is True
            0 in bool function is False
            Number 21 in binary is 0b10101
    * Вивів на екран роботу циклу та розгалужень в ньому
        ##### Код програми:
            Flip_flop = True
            for counter in range(4):
                if(Flip_flop):
                    print("Hello")
                    Flip_flop = False
                else:
                    print("there")
                    Flip_flop = True
        ##### Результат виконання:
            user@Pc:~/Python$ python3 trial.py 
            Hello
            there
            Hello
            there
    * Вивів на екран роботу конструкції try -> except -> finally
        ##### Код програми:
            x = 1
            try:
                num = input("Please enter a number: ")
                x = int(num)
            except ValueError as e:
                print("Oops!", num,"was no valid number.Try again...")
            finally:
                print("Problem finally found!")
        ##### Результат виконання:
            user@Pc:~/Python$ python3 trial.py 
            Please enter a number: f
            Oops! f was no valid number.Try again...
            Problem finally found!
    * Вивів на екран інфо з файлу через контекст-менеджер
        ##### Код програми:
            with open("text.txt", "r") as text:
                for line in text:
                    print(line)
        ##### Результат виконання:
            user@Pc:~/Python$ python3 trial.py 
            This text here is to test the "with" function
    * Ознайомився з Python lambdas
        ##### Код програми:
            test_lambda = lambda item: item+2
            var_number = 8
            print(test_lambda(var_number))
        ##### Результат виконання:
            user@Pc:~/Python$ python3 trial.py 
            10



