# BO_Energo
#Решение тестовых задач

#Первая задача. 
Условия задачи.
### Первое задание

Напишите сервис, который будет находить корни квадратного уравнения .Самостоятельно определите наиболее оптимальную структуру возвращаемых данных.


#Решение.

from math import *

a = float(input())

b = float(input())

c = float(input())

d = b**2-4*a*c

if d < 0:

    print('Нет корней')
    
elif d == 0:

    print(-b / (2*a))
    
elif d > 0:

    x1 = (-b - d ** 0.5) / (2*a)
    
    x2 = (-b + d ** 0.5) / (2*a)
    
    print(min(x1, x2))
    
    print(max(x1, x2))
    

Условие второй задачи.
### Второе задание

Есть группа из 100 предметов. 
Предметы могут быть синего, зелёного и красного цвета. 
Известно, что предметов синего цвета сильно больше, чем предметов зелёного цвета, а предметов зелёного цвета немного больше, чем предметов красного цвета. Напишите сервис, который будет принимать номер предмета и пытаться угадать его цвет. Логику работы сервиса определите самостоятельно.

#Решение Второй задачи.

#Вариантов раскладки количества предметов по цветам по формуле вероятности

#может быть 3 в степени 100 (получится число вариантов раскладки 100 предметов 

#по цветам).

#В нашей задаче мы используем один из вариантов раскладки по цветам с таким количеством: 

#синих предметов 55 штук,

#зеленых - 25 штук,

#красных - 20 штук,

#всего 100 штук по условию задачи.



a = int(input())

blue = 'синий'

green = 'зеленый'

red = 'красный'


    # предметы пронумерованные с 1 до 55 синий цвет (всего 55 штук предметов)
    
    
if 1<=a<=55:


    print(blue)
    

    # предметы пронумерованные с 56 по 80 зеленого цвета (всего 25 штук предметов)
    
    
elif 56<=a<=80:


    print(green)
    

    # предметы пронумерованные с 81 по 100 красного цвета (всего 20 штук)
    
    
elif 81<=a<=100 :


    print(red)
    
    
if a > 100 or a < 1:


    print('ошибка ввода')
    

