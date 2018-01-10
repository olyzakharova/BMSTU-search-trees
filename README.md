# search-trees

## Сравнение двух структур данных: красно-черного дерева (RBtree) и 2-3-дерева (23tree).
-------------------
## Список источников:
1. Томас Кормен, Чарльз Лейзерсон, Рональд Риверст, Клиффорд Штайн "Алгоритмы. Построение и анализ. Третье издание"
2. Ключарев П.Г. "Дополнительные главы дискретной математики: Алгоритмы и структуры данных"
3. http://cplusplus.kurttest.com
4. http://cs.wellesley.edu/~cs230/fall04/2-3-trees.pdf
5. http://cs.wellesley.edu/~cs231/fall01/red-black.pdf



### ПРИМЕЧАНИЕ: Тесты test1,test2,test3,test4,test5 написаны к обеим структурам данных. 
### Тесты test23_1-test23_4 и testRB1-testRB4 показывают, что программа и ее методы работают корректно.

# Входной файл с командами может содержать следующие команды:

***add [key] ***[data]

***delete [key]

***print

***search [key]

***max

***min

***(где key, data - целые числа)

# Описание команды print:


# Оценка сложности алгоритмов:
## Для 2-3-дерева:
1.	Вставка.
    Так как мы спускаемся один раз, и поднимаемся вверх при расщеплении родителей не более одного раза, то вставка работает за **O(log n)**;
2.	Поиск имеет сложность **O(log n)**;
3.	Удаление имеет сложность **O(log n)**.

## Для красно-черного дерева:
1.	Вставка имеет сложность **O(log n)**;
2.	Удаление имеет сложность **O(log n)**.
3.	Поиск имеет сложность **O(log n)**;

### НО

1.	Красно-черное дерево удаляет быстрее, хотя в 2-3-дереве при удалении количество подъемов не ограничено.
2.	Красно-черное дерево занимает меньше памяти.

# Сравнение:
 
В первой строке создаем дерево и поместили в него 1024 * 1024 элементов. 
Во второй строке мы по очереди ищем в дереве каждый из этих элементов.
В третьей строке удаляем из дерева по одному элементу.

# Результаты сравнения:
 
##  Для отсортированной последовательности:

2-3 tree:

Creation of tree with 1048576 nodes took **1141** ms

Finding all nodes took **199** ms

Deletion of all nodes took **295** ms

Red-Black tree:

Creation of tree with 1048576 nodes took **1093** ms

Finding all nodes took **219** ms

Deletion of all nodes took **280** ms


Исходя из этих данных можно сделать вывод, что: 
1. Вставка проходит быстрее в красно-черном дереве.
2. Поиск проходит быстрее в 2-3-дереве.
3. Удаление проходит быстрее в красно-черном дереве.

Но следует заметить, что разница очень невелика, так что теоретические ожидания почти подтвердились.

##  Для частично отсортированной последовательности:

2-3 tree:

Creation of tree with 1048576 nodes took **1141** ms

Finding all nodes took **199** ms

Deletion of all nodes took **295** ms

Red-Black tree:

Creation of tree with 1048576 nodes took **1093** ms

Finding all nodes took **219** ms

Deletion of all nodes took **280** ms


Исходя из этих данных можно сделать вывод, что: 
1. Вставка проходит быстрее в красно-черном дереве.
2. Поиск проходит быстрее в 2-3-дереве.
3. Удаление проходит быстрее в красно-черном дереве.

Но следует заметить, что разница очень невелика, так что теоретические ожидания почти подтвердились.


##  Для неотсортированной последовательности:

2-3 tree:

Creation of tree with 1048576 nodes took **1141** ms

Finding all nodes took **199** ms

Deletion of all nodes took **295** ms

Red-Black tree:

Creation of tree with 1048576 nodes took **1093** ms

Finding all nodes took **219** ms

Deletion of all nodes took **280** ms


Исходя из этих данных можно сделать вывод, что: 
1. Вставка проходит быстрее в красно-черном дереве.
2. Поиск проходит быстрее в 2-3-дереве.
3. Удаление проходит быстрее в красно-черном дереве.

Но следует заметить, что разница очень невелика, так что теоретические ожидания почти подтвердились.




