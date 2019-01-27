len() 统计字符串长度
可以使用lower（）方法除去字符串中的所有大小写。
upper()全部大写
string.lower()
string.upper()


<pre><code>name = raw_input("What is your name? ")
quest = raw_input("What is your quest? ")
color = raw_input("What is your favorite color? ")
#文字输入
</code></pre>

<pre><code>
print "Ah, so your name is %s, your quest is %s, " \
"and your favorite color is %s." % (name, quest, color)
</code></pre>


<pre><code>
from datetime import datetime
now = datetime.now()
print now
</code></pre>

输出
2019-01-21 02:13:03.534858

print '%02d-%02d-%04d' % (now.month, now.day, now.year)



<pre><code>
def clinic():
    print "You've just entered the clinic!"
    print "Do  you take the door on the left or the right?"
    answer = raw_input("Type left or right and hit 'Enter'.").lower()
    if answer == "left" or answer == "l":
        print "This is the Verbal Abuse Room, you heap of parrot droppings!"
    elif answer == "right" or answer == "r":
        print "Of course this is the Argument Room, I've told you that already!"
    else:
        print "You didn't pick left or right! Try again."
        clinic()

clinic()
</code></pre>

** 乘方


Python 格式 空格

.isalpha()

s[1:4] S字符串的第二到五位
  new_word = new_word[1:len(new_word)]


def one_good_turn(n):
  return n + 1
    
def deserves_another(n):
  return one_good_turn(n) + 2

sqrt()

from math import sqrt
from math import *


dir #get everything in the list

<pre><code>
print type(108)
print type(3.14)
print type('hello')
#各种类型支持
</code></pre>


赋值==

    def hotel_cost(night): #night变量
      return 140*night
    def hotel_cost(nights):
      return 140 * nights
    
<pre><code>
    def plane_ride_cost(city):
      if city == "Charlotte":
    return 183
      elif city == "Tampa":
    return 220
      elif city == "Pittsburgh":
    return 222
      elif city == "Los Angeles":
    return 475
</code></pre>
    
    def rental_car_cost(days):
      cost = days * 40
      if days >= 7:
    cost -= 50
      elif days >= 3:
    cost -= 20
      return cost

def trip_cost(city, days,spending_money):
  return rental_car_cost(days) + hotel_cost(days - 1) + plane_ride_cost(city)+spending_money

print trip_cost("Los Angeles",5,600)

letters.append(*)  #末尾添加，直接输入

letters[1:3]. #考虑1不考虑3

    my_list[:2]
    # 抓前两项
    my_list[3:]
    # 从第四项到最后一项

index 找寻项

    animals = ["aardvark", "badger", "duck", "emu", "fennec fox"]
    duck_index = animals.index("duck")# Use index() to find "duck"
    animals.insert(duck_index, "cobra")
    print animals # Observe what prints after the insert operation

for a in b   #a给予一个元素统称在B中
.sort 排序

<pre><code>
    residents = {'Puffin' : 104, 'Sloth' : 105, 'Burmese Python' : 106}
    #变量值
</code></pre>


    dict_name[new_key] = new_value  #添加元素
    del dict_name[key_name] #删除元素  {}
    
    list.remove(element) #删除元素
    
    inventory['backpack'].remove('dagger')
    
    inventory['pocket'] = ['seashell', 'strange berry', 'lint']
    inventory['backpack'].sort()
    inventory['backpack'].remove('dagger')
    inventory['gold'] = inventory['gold'] + 50

<pre><code>
for a in webster:
  print webster[a]
# 子内容选择
</code></pre>

% 2 == 0 #偶数测试方法

    prices = {"banana": 4,"apple": 2,"orange": 1.5,"pear": 3}
    stock = {"banana": 6,"apple": 0,"orange": 32,"pear": 15}
    for a in prices:
      print a
      print "price: %s" % prices[a]
      print "stock: %s" % stock[a]

<pre><code>
lloyd = {
  "name": "Lloyd",
  "homework": [90.0, 97.0, 75.0, 92.0],
  "quizzes": [88.0, 40.0, 94.0],
  "tests": [75.0, 90.0]
}
alice = {
  "name": "Alice",
  "homework": [100.0, 92.0, 98.0, 100.0],
  "quizzes": [82.0, 83.0, 91.0],
  "tests": [89.0, 97.0]
}
tyler = {
  "name": "Tyler",
  "homework": [0.0, 87.0, 75.0, 22.0],
  "quizzes": [0.0, 75.0, 78.0],
  "tests": [100.0, 100.0]
}

# Add your function below!
def average(numbers):
  total = sum(numbers)
  total = float(total)
  return total/len(numbers)

def get_average(student):
  homework = average(student["homework"])
  quizzes = average(student["quizzes"])
  tests = average(student["tests"])
  return 0.1 * homework + 0.3 * quizzes + 0.6 * tests

def get_letter_grade(score):
  if score >= 90:
return "A"
  elif score >=80:
return "B"
  elif score >=70:
return "C"
  elif score >=60:
return "D"
  else:
return "F"

def get_class_average(class_list):
  results = []
  for student in class_list:
student_avg = get_average(student)
results.append(student_avg)
  return average(results)

students = [lloyd, alice, tyler]

avg = get_class_average(students)
print(avg)
print(get_letter_grade(avg))

#平均成绩
</code></pre>

    
    range(stop)
    range(start, stop)
    range(start, stop, step)
    
    n = [[1, 2, 3], [4, 5, 6, 7, 8, 9]]
    
    def flatten(lists):
      results = []
      for numbers in lists:
    for number in numbers:
      results.append(number)
      return results
    
    print flatten(n)
    #合并数组

