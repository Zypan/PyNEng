##Синтаксис Python

Первое, что, как правило, бросается в глаза, если говорить о синтаксисе Python, это то, что отступы имеют значение:
* они определяют какие выражения попадают в блок кода
* когда блок кода заканчивается

Кто-то за это Python любит, кто-то нет.

Посмотрим на пример кода:
```python
a = 10
b = 5

if a > b:
    print "A больше B"
    print "Тут можно выполнить ещё что-то"
else:
    print "B больше или равно A"
    print "Продолжаем тут же"

print "The End"
```

Несмотря на то, что мы еще не разбирались с инструкцией if/else, всё должно быть понятно.

Python понимает какие строки относятся к if на основе отступов. Выполнение части ```if a > b``` заканчивается тогда, когда мы попадаем на строку с тем же отступом, что и сама строка ```if a > b```.

Аналогично с блоком else.

Вторая особенность, которую мы тут видим: после некоторых выражений должно идти двоеточие (например, после if a > b или после else).

Несколько правил:
* В качестве отступов могут использоваться Tab или пробелы. 
  * лучше использовать пробелы
    * дело в том, что в некоторых редакторах таб может превращаться в пробелы, в в других нет. И, чтобы избежать неразберихи, лучше стразу использовать пробелы.
* Количество пробелов должно быть одинаковым в одном блоке.
  * лучше чтобы количество пробелов было одинаковым во всем коде
  * популярный вариант использовать 3-4 пробела

> **Note** Для того чтобы проблем с отступами не было, надо сразу настроить редактор таким образом, чтобы отступы делались автоматически.

> Редактор должен поддерживать Python. И, скорее всего, подгрузив поддержку Python принятым в редакторе способом, вы получите авто отступы сразу.

Еще одна особенность приведенного примера кода: пустые строки. Таким образом мы просто наводим красоту в коде.

Правда предыдущий вариант более приятно читать, чем этот?
```python
a = 10
b = 5
if a > b:
    print "A больше B"
    print "Тут можно выполнить ещё что-то"
else:
    print "B больше или равно A"
    print "Продолжаем тут же"
print "The End"
```

Остальные особенности синтаксиса мы будем изучать в процессе знакомства с структурами данных в Python.

###Комментарии

Комментарии в Python могут быть однострочными:
```python
#Очень важный комментарий
a = 10
b = 5 #Очень нужный комментарий
```
Однострочные комментарии начинаются со знака #.

Обратите внимание, что коментарий может быть и в строке где находится код, и сам по себе.

Если же вам нужно написать несколько строк комментария, то, чтобы не ставить перед кажой решетку, можно сделать многострочный комметарий:
```python
"""Очень важный комментарий
и длинный комментарий
"""
a = 10
b = 5
```

Комментарии могут использоваться как для того, чтобы комментировать, что происходит в коде, так и для того, чтобы закомментировать временно какое-то выражение.