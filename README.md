# search-trees

## Сравнение двух структур данных: красно-черного дерева (RBtree) и 2-3-дерева (23tree).

## Список источников:
1. Томас Кормен, Чарльз Лейзерсон, Рональд Риверст, Клиффорд Штайн "Алгоритмы. Построение и анализ. Третье издание"
2. Ключарев П.Г. "Дополнительные главы дискретной математики: Алгоритмы и структуры данных"
3. http://cplusplus.kurttest.com
4. http://cs.wellesley.edu/~cs230/fall04/2-3-trees.pdf
5. http://cs.wellesley.edu/~cs231/fall01/red-black.pdf



Тесты test1,test2,test3,test4,test5 написаны к обеим структурам данных.

# Входной файл с командами может содержать следующие команды:

add [key] [data]

delete [key]

print

search [key]

max

min

postorder

preorder

inorder

где key, data - целые числа.




# Результаты сравнения:

2-3 tree:
Creation of tree with 1048576 nodes took 1878ms
Finding all nodes took 510ms

Red-Black tree:
Creation of tree with 1048576 nodes took 1049ms
Finding all nodes took 366ms
