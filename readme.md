# 🐍 30 Days Of Python 

|# Day | Topics                                                    |
|------|:---------------------------------------------------------:|
| 01  |  [Introduction](./readme.md)|
| 02  |  [Variables, Built-in Functions](./02_Day_Variables_builtin_functions/02_variables_builtin_functions.md)|
| 03  |  [Operators](./03_Day_Operators/03_operators.md)|
| 04  |  [Strings](./04_Day_Strings/04_strings.md)|
| 05  |  [Lists](./05_Day_Lists/05_lists.md)|
| 06  |  [Tuples](./06_Day_Tuples/06_tuples.md)|
| 07  |  [Sets](./07_Day_Sets/07_sets.md)|
| 08  |  [Dictionaries](./08_Day_Dictionaries/08_dictionaries.md)|
| 09  |  [Conditionals](./09_Day_Conditionals/09_conditionals.md)|
| 10  |  [Loops](./10_Day_Loops/10_loops.md)|
| 11  |  [Functions](./11_Day_Functions/11_functions.md)|
| 12  |  [Modules](./12_Day_Modules/12_modules.md)|
| 13  |  [List Comprehension](./13_Day_List_comprehension/13_list_comprehension.md)|
| 14  |  [Higher Order Functions](./14_Day_Higher_order_functions/14_higher_order_functions.md)|     
| 15  |  [Python Type Errors](./15_Day_Python_type_errors/15_python_type_errors.md)| 
| 16 |  [Python Date time](./16_Day_Python_date_time/16_python_datetime.md) |     
| 17 |  [Exception Handling](./17_Day_Exception_handling/17_exception_handling.md)|    
| 18 |  [Regular Expressions](./18_Day_Regular_expressions/18_regular_expressions.md)|    
| 19 |  [File Handling](./19_Day_File_handling/19_file_handling.md)|
| 20 |  [Python Package Manager](./20_Day_Python_package_manager/20_python_package_manager.md)|
| 21 |  [Classes and Objects](./21_Day_Classes_and_objects/21_classes_and_objects.md)|
| 22 |  [Web Scraping](./22_Day_Web_scraping/22_web_scraping.md)|
| 23 |  [Virtual Environment](./23_Day_Virtual_environment/23_virtual_environment.md)|
| 24 |  [Statistics](./24_Day_Statistics/24_statistics.md)|
| 25 |  [Pandas](./25_Day_Pandas/25_pandas.md)|
| 26 |  [Python web](./26_Day_Python_web/26_python_web.md)|
| 27 |  [Python with MongoDB](./27_Day_Python_with_mongodb/27_python_with_mongodb.md)|
| 28 |  [API](./28_Day_API/28_API.md)|
| 29 |  [Building API](./29_Day_Building_API/29_building_API.md)|
| 30 |  [Conclusions](./30_Day_Conclusions/30_conclusions.md)|

<div align="center">
  <h1> 30 Days Of Python: Day 1 - Introduction</h1>
  <sub>
    Author: <a href="https://www.linkedin.com/in/asabeneh/" target="_blank">Asabeneh Yetayeh</a><br>
    Dịch: Đặng Quang Minh <br>
  </sub>
</div>

- [📘 Day 1](#-day-1)
  - [Virtualenv](#virtualenv)
  - [Environment Setup](#environment-setup)
    - [Virtualenv](#virtualenv)
    - [Python Shell](#python-shell)
    - [Installing Visual Studio Code](#installing-visual-studio-code)
      - [How to use visual studio code](#how-to-use-visual-studio-code)
  - [Basic Python](#basic-python)
    - [Python Syntax](#python-syntax)
    - [Python Indentation](#python-indentation)
    - [Comments](#comments)
    - [Data types](#data-types)
      - [Number](#number)
      - [String](#string)
      - [Booleans](#booleans)
      - [List](#list)
      - [Dictionary](#dictionary)
      - [Tuple](#tuple)
      - [Set](#set)
    - [Checking Data types](#checking-data-types)
    - [Python File](#python-file)
  - [💻 Exercises - Day 1](#-exercises---day-1)
    - [Exercise: Level 1](#exercise-level-1)
    - [Exercise: Level 2](#exercise-level-2)
    - [Exercise: Level 3](#exercise-level-3)

# 📘 Day 1

## Environment Setup

### Virtualenv

Cài đặt virtualenv trên MacOS

```
$ brew install virtualenv
```

Tạo một môi trường mới

```
$ virtualenv <tên môi trường>
```

Tạo một môi trường mới với phiên bản python cố định nào đó

```
$ virtualenv -p python3.10 <tên môi trường>
```

Install python theo phiên bản cố định nào đó

```
$ brew install python@<version-muốn-cài>
```

### Python Shell

Python là một ngôn ngữ script thông dịch, nó không cần phải biên dịch.\
Có nghĩa là nó sẽ thực thi dòng code line by line.\
Python cung cấp Python Shell, nó dùng để thực thi từng câu lệnh đơn lẻ và trả về luôn kết quả.

Python Shell đợi user gõ code. Sau khi user nhập lệnh code, nó sẽ thông dịch code và hiển thị kết quả vào dòng kế tiếp.\
Mở terminal lên, rồi gõ câu lệnh phía dưới:

```shell
$ python
```

![Python Scripting Shell](./images/opening_python_shell.png)

The Python interactive shell sẽ được mở ra, và nó đợi bạn viết code Python vào đấy.

You will write your Python script next to this symbol >>> and then click Enter.\
Bạn sẽ gõ code python vào sau 3 ký tự >>> rồi bấm Enter.\
Hãy xem tôi gõ dòng code đầu tiên vào Python scripting shell.

![Python script on Python shell](./images/adding_on_python_shell.png)

Bùm, bạn đã viết đoạn mã python đầu tiên vào Python interactive shell.\
Rồi, để tắt cái sheel này đi, gõ lệnh **exit()** rồi bấm Enter.

![Exit from python shell](./images/exit_from_shell.png)

Yeah, giờ bạn đã biết cách open một Python interactive shell và biết cách tắt nó đi.

Python sẽ cho bạn kết quả nếu đoạn code bạn viết là đúng, nếu sai nó sẽ trả về errors.\
Hãy cùng tôi cố ý tạo ra một lỗi và xem Python nó trả về cái gì.

![Invalid Syntax Error](./images/invalid_syntax_error.png)

Quá trình xác nhận và loại bỏ errors trong chương trình được gọi là *debugging*.\
Chúng ta debug nó bằng cách thay đổi **x** thành *.

![Fixing Syntax Error](./images/fixing_syntax_error.png)

Bug đã được fix, chương trình chạy và chúng ta nhận được kết quả như mong đợi.\
Như một lập trình viên, bạn sẽ ngập trong errors ngày qua ngày.\
Bạn sẽ phải fix nó. Để giỏi trong debugging, bạn cần hiểu những loại lỗi mà bạn gặp.\
Một vài lỗi trong Python là: *SyntaxError*, *IndexError*, *NameError*, *ModuleNotFoundError*, *KeyError*, *ImportError*, *AttributeError*, *TypeError*, *ValueError*, *ZeroDivisionError* etc. \
Chúng ta sẽ xem khác biệt giữa các loại lỗi trong Python trong sessions sau.

Chúng ta hãy luyện thêm cách sử dụng Python shell. Mở terminal lên và gõ **python**.

![Python Scripting Shell](./images/opening_python_shell.png)

The Python interactive shell được mở lên.\
Chúng ta hãy thực hiện một vài toán tử (cộng trừ nhân chia, lấy phần dư, số mũ (exponential))

Chúng ta thực hiện vài pheps toán đơn giản trước khi viết bất kỳ python code nào:

- 2 + 3 = 5
- 3 - 2 = 1
- 3 \* 2 = 6
- 3 / 2 = 1.5
- 3 ^ 2 = 3 x 3 = 9

Trong python, chúng ta có một vài toán tử bổ sung:

- 3 % 2 = 1 => có nghĩa là tìm phần còn lại
- 3 // 2 = 1 => có nghĩa là loại bỏ phần còn lại

Let us change the above mathematical expressions to Python code. The Python shell has been opened and let us write a comment at the very beginning of the shell.

Chúng ta thay đổi cú pháp toán bên trong Python code. Python shell đã mở ra trước đó, và chúng ta viết comment tại điểm bắt đầu của shell.

A _comment_ is a part of the code which is not executed by python. So we can leave some text in our code to make our code more readable. Python does not run the comment part. A comment in python starts with hash(#) symbol.
This is how you write a comment in python

```shell
 # comment starts with hash
 # this is a python comment, because it starts with a (#) symbol
```

![Maths on python shell](./images/maths_on_python_shell.png)

Before we move on to the next section, let us practice more on the Python interactive shell. Close the opened shell by writing _exit()_ on the shell and open it again and let us practice how to write text on the Python shell.

![Writing String on python shell](./images/writing_string_on_shell.png)

### Installing Visual Studio Code

The Python interactive shell is good to try and test small script codes but it will not be for a big project. In real work environment, developers use different code editors to write codes. In this 30 days of Python programming challenge we will use visual studio code. Visual studio code is a very popular open source text editor. I am a fan of vscode and I would recommend to [download](https://code.visualstudio.com/) visual studio code, but if you are in favor of other editors, feel free to follow with what you have.

[![Visual Studio Code](./images/vscode.png)](https://code.visualstudio.com/)

If you installed visual studio code, let us see how to use it.
If you prefer a video, you can follow this Visual Studio Code for Python [Video tutorial](https://www.youtube.com/watch?v=bn7Cx4z-vSo)

#### How to use visual studio code

Open the visual studio code by double clicking the visual studio icon. When you open it you will get this kind of interface. Try to interact with the labeled icons.

![Visual studio Code](./images/vscode_ui.png)

Create a folder named 30DaysOfPython on your desktop. Then open it using visual studio code.

![Opening Project on Visual studio](./images/how_to_open_project_on_vscode.png)

![Opening a project](./images/opening_project.png)

After opening it you will see shortcuts for creating files and folders inside of 30DaysOfPython project's directory. As you can see below, I have created the very first file, helloworld.py. You can do the same.

![Creating a python file](./images/helloworld.png)

After a long day of coding, you want to close your code editor, right? This is how you will close the opened project.

![Closing project](./images/closing_opened_project.png)

Congratulations, you have finished setting up the development environment. Let us start coding.

## Basic Python

### Python Syntax

A Python script can be written in Python interactive shell or in the code editor. A Python file has an extension .py.

### Python Indentation

An indentation is a white space in a text. Indentation in many languages is used to increase code readability, however Python uses indentation to create block of codes. In other programming languages curly brackets are used to create blocks of codes instead of indentation. One of the common bugs when writing python code is wrong indentation.

![Indentation Error](./images/indentation.png)

### Comments

Comments are very important to make the code more readable and to leave remarks in our code. Python does not run comment parts of our code.
Any text starting with hash(#) in Python is a comment.

**Example: Single Line Comment**

```shell
    # This is the first comment
    # This is the second comment
    # Python is eating the world
```

**Example: Multiline Comment**

Triple quote can be used for multiline comment if it is not assigned to a variable

```shell
"""This is multiline comment
multiline comment takes multiple lines.
python is eating the world
"""
```

### Data types

In Python there are several types of data types. Let us get started with the most common ones. Different data types will be covered in detail in other sections. For the time being, let us just go through the different data types and get familiar with them. You do not have to have a clear understanding now.

#### Number

- Integer: Integer(negative, zero and positive) numbers
    Example:
    ... -3, -2, -1, 0, 1, 2, 3 ...
- Float: Decimal number
    Example
    ... -3.5, -2.25, -1.0, 0.0, 1.1, 2.2, 3.5 ...
- Complex
    Example
    1 + j, 2 + 4j

#### String

A collection of one or more characters under a single or double quote. If a string is more than one sentence then we use a triple quote.

**Example:**

```py
'Asabeneh'
'Finland'
'Python'
'I love teaching'
'I hope you are enjoying the first day of 30DaysOfPython Challenge'
```

#### Booleans

A boolean data type is either a True or False value. T and F should be always uppercase.

**Example:**

```python
    True  #  Is the light on? If it is on, then the value is True
    False # Is the light on? If it is off, then the value is False
```

#### List

Python list is an ordered collection which allows to store different data type items. A list is similar to an array in JavaScript.

**Example:**

```py
[0, 1, 2, 3, 4, 5]  # all are the same data types - a list of numbers
['Banana', 'Orange', 'Mango', 'Avocado'] # all the same data types - a list of strings (fruits)
['Finland','Estonia', 'Sweden','Norway'] # all the same data types - a list of strings (countries)
['Banana', 10, False, 9.81] # different data types in the list - string, integer, boolean and float
```

#### Dictionary

A Python dictionary object is an unordered collection of data in a key value pair format. 

**Example:**

```py
{
'first_name':'Asabeneh',
'last_name':'Yetayeh',
'country':'Finland', 
'age':250, 
'is_married':True,
'skills':['JS', 'React', 'Node', 'Python']
}
```

#### Tuple

A tuple is an ordered collection of different data types like list but tuples can not be modified once they are created. They are immutable.

**Example:**

```py
('Asabeneh', 'Pawel', 'Brook', 'Abraham', 'Lidiya') # Names
```

```py
('Earth', 'Jupiter', 'Neptune', 'Mars', 'Venus', 'Saturn', 'Uranus', 'Mercury') # planets
```

#### Set

A set is a collection of data types similar to list and tuple. Unlike list and tuple, set is not an ordered collection of items. Like in Mathematics, set in Python stores only unique items.

In later sections, we will go in detail about each and every Python data type.

**Example:**

```py
{2, 4, 3, 5}
{3.14, 9.81, 2.7} # order is not important in set
```

### Checking Data types

To check the data type of certain data/variable we use the **type** function. In the following terminal you will see different python data types:

![Checking Data types](./images/checking_data_types.png)

### Python File

First open your project folder, 30DaysOfPython. If you don't have this folder, create a folder name called 30DaysOfPython. Inside this folder, create a file called helloworld.py. Now, let's do what we did on python interactive shell using visual studio code.

The Python interactive shell was printing without using **print** but on visual studio code to see our result we should use a built in function *print(). The *print()* built-in function takes one or more arguments as follows *print('arument1', 'argument2', 'argument3')*. See the examples below.

**Example:**

The file name is helloworld.py

```py
# Day 1 - 30DaysOfPython Challenge

print(2 + 3)             # addition(+)
print(3 - 1)             # subtraction(-)
print(2 * 3)             # multiplication(*)
print(3 / 2)             # division(/)
print(3 ** 2)            # exponential(**)
print(3 % 2)             # modulus(%)
print(3 // 2)            # Floor division operator(//)

# Checking data types
print(type(10))          # Int
print(type(3.14))        # Float
print(type(1 + 3j))      # Complex number
print(type('Asabeneh'))  # String
print(type([1, 2, 3]))   # List
print(type({'name':'Asabeneh'})) # Dictionary
print(type({9.8, 3.14, 2.7}))    # Set
print(type((9.8, 3.14, 2.7)))    # Tuple
```

To run the python file check the image below. You can run the python file either by running the green button on Visual Studio Code or by typing *python helloworld.py* in the terminal .

![Running python script](./images/running_python_script.png)

🌕  You are amazing. You have just completed day 1 challenge and you are on your way to greatness. Now do some exercises for your brain and muscles.

## 💻 Exercises - Day 1

### Exercise: Level 1

1. Check the python version you are using
2. Open the python interactive shell and do the following operations. The operands are 3 and 4.
   - addition(+)
   - subtraction(-)
   - multiplication(\*)
   - modulus(%)
   - division(/)
   - exponential(\*\*)
   - floor division operator(//)
3. Write strings on the python interactive shell. The strings are the following:
   - Your name
   - Your family name
   - Your country
   - I am enjoying 30 days of python
4. Check the data types of the following data:
   - 10
   - 9.8
   - 3.14
   - 4 - 4j
   - ['Asabeneh', 'Python', 'Finland']
   - Your name
   - Your family name
   - Your country

### Exercise: Level 2

1. Create a folder named day_1 inside 30DaysOfPython folder. Inside day_1 folder, create a python file helloworld.py and repeat questions 1, 2, 3 and 4. Remember to use _print()_ when you are working on a python file. Navigate to the directory where you have saved your file, and run it.

### Exercise: Level 3

1. Write an example for different Python data types such as Number(Integer, Float, Complex), String, Boolean, List, Tuple, Set and Dictionary.
2. Find an [Euclidian distance](https://en.wikipedia.org/wiki/Euclidean_distance#:~:text=In%20mathematics%2C%20the%20Euclidean%20distance,being%20called%20the%20Pythagorean%20distance.) between (2, 3) and (10, 8)

🎉 Chúc mừng nhé bro ! 🎉

[Day 2 >>](./02_Day_Variables_builtin_functions/02_variables_builtin_functions.md)