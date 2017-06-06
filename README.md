# aMAZEd

Implementation of Maze algorithms

Python implementation of the algorithms presented in the book [Mazes for Programmers][REF1] by Jamis Buck

## Binary Tree Method

```sh
$ python binary_tree.py
Enter number of rows: 8
Enter number of columns: 14
+---+---+---+---+---+---+---+---+---+---+---+---+---+---+
|                                                       |
+   +   +---+---+   +   +---+   +   +   +---+---+   +   +
|   |   |           |   |       |   |   |           |   |
+   +   +---+   +   +   +---+---+---+---+---+---+---+   +
|   |   |       |   |   |                               |
+---+---+---+---+---+   +---+   +   +   +---+---+   +   +
|                       |       |   |   |           |   |
+---+---+---+   +---+---+---+   +   +---+   +---+   +   +
|               |               |   |       |       |   |
+---+   +---+   +---+---+---+---+   +---+---+   +   +   +
|       |       |                   |           |   |   |
+---+   +---+---+   +   +---+   +---+   +   +---+---+   +
|       |           |   |       |       |   |           |
+---+   +   +   +---+---+---+---+---+---+   +---+   +   +
|       |   |   |                           |       |   |
+---+---+---+---+---+---+---+---+---+---+---+---+---+---+

```

## Sidewinder Algorithm

```sh
$ python sidewinder.py -h
usage: sidewinder.py [-h] [-d | -g] r c

positional arguments:
  r                    Number of rows
  c                    Number of columns

optional arguments:
  -h, --help           show this help message and exit
  -d, --distance_grid
  -g, --grid

$ python sidewinder.py -g 6 8
+---+---+---+---+---+---+---+---+
|                               |
+   +---+---+---+---+---+---+   +
|           |                   |
+---+---+   +   +   +---+   +---+
|           |   |   |           |
+---+---+---+   +---+   +---+   +
|                   |   |       |
+---+   +---+   +---+   +---+---+
|       |           |           |
+---+   +---+---+---+---+---+---+
|                               |
+---+---+---+---+---+---+---+---+

$ python sidewinder.py -d 6 12
+---+---+---+---+---+---+---+---+---+---+---+---+
|  0   1   2   3   4   5   6   7   8   9  10  11|
+---+---+   +   +---+   +   +   +---+   +---+---+
|  5   4   3|  4   5|  6|  7|  8| 11  10  11  12|
+   +---+   +---+---+---+---+---+---+---+---+---+
|  6|  5   4   5   6   7   8   9  10  11  12  13|
+---+---+   +---+---+---+---+---+---+---+---+   +
|  7   6   5   6   7   8   9  10| 17  16  15  14|
+---+---+---+   +   +---+---+   +---+   +   +   +
| 10   9   8   7|  8   9  10| 11| 18  17| 16| 15|
+---+   +---+   +---+   +---+---+---+   +   +---+
| 11  10  11|  8| 11  10| 21  20  19  18| 17  18|
+---+---+---+---+---+---+---+---+---+---+---+---+

```

## Aldous-broder Method

```sh
$ python aldous_broder.py -g 10 12
+---+---+---+---+---+---+---+---+---+---+---+---+
|                   |           |   |   |       |
+   +---+   +   +---+---+   +---+   +   +   +---+
|   |       |   |       |   |       |   |       |
+   +   +---+---+   +   +   +   +---+   +---+   +
|   |       |       |   |       |               |
+   +---+---+   +---+---+   +---+---+   +   +---+
|           |                   |       |       |
+---+   +   +   +---+   +   +   +   +---+---+   +
|       |   |       |   |   |           |   |   |
+---+---+   +   +   +   +   +   +---+---+   +   +
|   |           |   |   |   |   |               |
+   +   +---+---+---+   +---+---+   +   +   +---+
|   |   |       |               |   |   |       |
+   +---+---+   +---+---+   +---+---+   +---+   +
|                           |   |   |   |       |
+---+   +---+---+   +---+   +   +   +   +---+---+
|           |       |       |   |               |
+   +---+   +---+---+---+---+   +---+   +---+---+
|   |                           |               |
+---+---+---+---+---+---+---+---+---+---+---+---+
```

## Wilson's Algorithm

```sh
$ python wilson.py -g 8 12
+---+---+---+---+---+---+---+---+---+---+---+---+
|   |                       |       |   |       |
+   +   +---+   +---+---+   +   +---+   +   +   +
|       |       |       |   |   |       |   |   |
+---+   +---+   +---+   +---+   +   +---+   +   +
|           |   |           |       |   |   |   |
+   +---+   +   +---+   +   +   +---+   +---+   +
|   |       |   |   |   |   |   |           |   |
+---+   +---+   +   +   +   +   +---+   +   +   +
|   |   |               |           |   |       |
+   +---+---+---+   +---+   +---+---+---+   +---+
|           |   |       |                   |   |
+---+---+   +   +---+   +---+   +   +   +   +   +
|   |                       |   |   |   |   |   |
+   +   +---+---+---+---+---+   +   +---+---+   +
|                   |           |               |
+---+---+---+---+---+---+---+---+---+---+---+---+

```
License
----
MIT

[REF1]: https://www.amazon.com/Mazes-Programmers-Twisty-Little-Passages/dp/1680500554

