# Графы

**Граф** состоит из вершин, соединенных ребрами.Мы будем обозначать буквой n  количество вершин, а буквой m - количество ребер
Вершины нумеруются числами от 1 до n.

На рисунке изображен граф с 5 вершинами и 7 ребрами

![](images/graph_1.jpeg)


### Основные определения:

- **Смежные вершины** - это вершины, которые соединены ребром

- **Степень вершины** - это количество ребер исходящих из вершины

- Ребро (1, 2) **инцидентно** вершинам 1 и 2

- **Кратные ребра** - это ребра, которые соединяют одну и ту же пару вершин.

- **Петля** - это ребро, которое соединяет вершину саму с собой

- **Простой граф** - это граф, который не содержит петель и кратных ребер.

- **Взвешенный граф** - это граф каждому ребру которого присвоено некоторое вещественное число называемое весом ребра

- **Ориентированный граф**  - граф, ребра которого имеют направление

- **Связный граф** - это граф с каждой вершины которого можно попасть в каждую


## Способы хранения графа.
Всего есть три способа:
1. **Матрица смежности** - матрица NxN элементов из нулей и единичек, где N - количество вершин.
a[i][j] элемент матрицы равен 1, если вершины i и j смежны.
2. **Список ребер** - буквально список из пар рёбер.(`std:vector<pair<int, int>>`)
3. **Список смежности** - двумерный вектор, где первый индекс i это номер вершины, а вектор по данному индексу - это список номеров смежных вершин.

