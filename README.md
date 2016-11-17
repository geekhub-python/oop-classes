### Задание 1

Напишите класс Temperature который по умолчанию при инициализации принимает температуру в градусах по цельсию. А его строковое представление(```__str__```) возвращает температура по цельсию и фарангейту. Отдельно для этого класса можно установить температуру по фарангейту через setter "fahrenheit"

 	
	In: temperature = Temperature(24)
	In: print(temperature)
	Out: Celsius: 24
	Fahrenheit: 75.2
	
	In: temperature.celsius = 10
	In: print(temperature)
	Out: Celsius: 10
	Fahrenheit: 50

    In: temperature.fahrenheit = 100
    In: print(temperature)
    Out: Celsius: 37.7778
	Fahrenheit: 100  

  
### Задание 2

Создайте класс, описывающий книгу. Он должен содержать информацию об авторе,
названии, годе издания и жанре. Создайте несколько разных книг. Определите
для него операции проверки на равенство и неравенство, методы ```__repr__``` и ```__str__```.


	In: orwell1984 = Book('George Orwell', '1984', 1949, 'dystopia')
	In: orwell_copy = copy.copy(orwell1984)  # копирование объекта
	In: learning_python = Book('Mark Lutz', 'Learning Python', 2013, 'tutorial')

    In: print(orwell1984)
    Out: "1984" by George Orwell (published in 1949, genre: dystopia)
    In: print(learning_python)
    Out: "Learning Python" by Mark Lutz (published in 2013, genre: tutorial)
    In: print(repr(orwell1984))
    Out: Book('George Orwell', '1984', 1949, 'dystopia')
    In: print(repr(learning_python))
    Out: Book('Mark Lutz', 'Learning Python', 2013, 'tutorial')
    
    In: print(orwell1984 == orwell_copy)
    True
    In: print(orwell1984 != orwell_copy)
    True
    In: print(orwell1984 == learning_python)
    False
    In: print(orwell1984 != learning_python)
    True
    In: print(learning_python == learning_python)
    True
    In: print(learning_python != learning_python)
    False
    