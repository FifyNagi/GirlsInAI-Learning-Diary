## Day 3 Viariables
### Log:
1. Assign values to variables  
2. Using the function `print()` and operator **+** with numbers(objects)  
3. Reading Materials:   
- [x] [Reading 1](https://www.tutorialspoint.com/python3/python_variable_types.htm)
- [ ] [Reading 2](https://docspy3zh.readthedocs.io/en/latest/reference/datamodel.html)  
- [ ] [Something I don't quite understand now](https://stackoverflow.com/questions/1436703/difference-between-str-and-repr)

### Note:
* Variables are reserved memory locations to store values
* & is a bitwise operator and it's not a substitute for + and not used to combine texts (+ is used to connect two strings)
* & is used to test odd and even numbers
![& in python](https://github.com/FifyNagi/GirlsInAI-Learning-Diary/blob/master/Others/%26%20in%20python.png)
![& in python 2](https://github.com/FifyNagi/GirlsInAI-Learning-Diary/blob/master/Others/%26%20in%20python%202.png)

![Homework3-1](https://github.com/FifyNagi/GirlsInAI-Learning-Diary/blob/master/Others/homework3-1.png)
![Homework3-2](https://github.com/FifyNagi/GirlsInAI-Learning-Diary/blob/master/Others/homework3-2.png)

***
### Reading 1
* Assigning same value to different variables  
`a=b=c=1`
* Assigning multiple variables at same time  
`a, b=1, "Apple"`
* Deleting variables using del  
`del a, b`
* Python have 5 standard data types
  * Numbers (int, float, complex)
  * String
  ```
  #!/usr/bin/python3
  
  str = 'Hello World!'
  
  print (str)          # Prints complete string
  print (str[0])       # Prints first character of the string
  print (str[2:5])     # Prints characters starting from 3rd to 5th
  print (str[2:])      # Prints string starting from 3rd character
  print (str * 2)      # Prints string two times
  print (str + "TEST") # Prints concatenated string
  ```
  * List
  ```
  #!/usr/bin/python3
  
  list = [ 'abcd', 786 , 2.23, 'john', 70.2 ]
  tinylist = [123, 'john']
  
  print (list)          # Prints complete list
  print (list[0])       # Prints first element of the list
  print (list[1:3])     # Prints elements starting from 2nd till 3rd 
  print (list[2:])      # Prints elements starting from 3rd element
  print (tinylist * 2)  # Prints list two times
  print (list + tinylist) # Prints concatenated lists
  ```
  * Tuple (read-only lists)
	Strings, numbers and tuples are immutable, when you change the assigned value, the [id changed](https://www.youtube.com/watch?v=LTw5-5tx5wg)  
	不可更改貌似是为了hashed.如果修改key那么hash function就不能用了？不是很懂  
	大多数情况下, 当我们谈及一个容器的值时, 指的只是值, 而不是被包含对象的标识符. 但是, 当我们谈及容器对象可变性的时候, 指的就是被直接包含的对象的标识了. 因此, 如果一个不可变对象 (如元组) 包含了可变对象, 只要这个可变对象的值变了则容器的值就也改变了  
  ```
  #!/usr/bin/python3
  
  tuple = ( 'abcd', 786 , 2.23, 'john', 70.2  )
  list = [ 'abcd', 786 , 2.23, 'john', 70.2  ]
  tuple[2] = 1000    # Invalid syntax with tuple
  list[2] = 1000     # Valid syntax with list
  ```
  * Dictionary (keys and values; **no order**)
  ![Dictionary](https://github.com/FifyNagi/GirlsInAI-Learning-Diary/blob/master/Others/dictionary.png)
* Data Type conversion: use the type-names as a function (`a="90.3"`, `b=float(a)`)  
a is a string and b is a float
