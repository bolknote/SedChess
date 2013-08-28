## Шахматы, написанные на языке утилиты sed / Chess implemented in sed utility

English guide is below

### Запуск
sed -f chess.sed

### Инструкция
Для начала нажите `Enter`. Чтобы выйти, нажмите `q`, затем `Enter`.

Чтобы сделать ход, введите его через пробел, затем `Enter`, например: `e2 e4`. Вы ходите белыми.

### Реализовано:
1. позиционная оценка на один ход и оценка фигур
2. обнаружение шаха и мата
3. прошедшая пешка преобразуется в ферзя

### Не реализовано:
1. рокировка (введена в правила в XIV-XV вв.)
2. взятие на проходе (введено в XV в)
3. обнаружение пата
4. контроль за правильностью хода человека

### Решения проблем
- sed: file chess.sed line 312: strings for `y' command are different lengths

Убедитесь, что ваша консоль использует локаль UTF-8 (например, ru_RU.UTF-8)

## English

### Launch
sed -f chess.sed

### How to play
Press `Enter` to start. Press `q` and `Enter` to quit.

To make a turn write it down separated by a space, then press `Enter`. For example: `e2 e4`. You play white side.

### Implemented
1. Position evaluation for one turn and pieces evaluation.
2. Detection of check and checkmate.
3. A pawn that reaches the opposite side promotes to a queen.

### Not implemented
1. Castling (introduced in 14-15th century rules)
2. En passant (introduced in 15th century rules)
3. Detection of stalemate
4. Controlling correctness of human moves

### Troubleshooting

- sed: file chess.sed line 312: strings for `y' command are different lengths

  [Make sure you are using a UTF locale
  (e.g. en_US.UTF-8)](https://github.com/bolknote/SedChess/issues/9)


-- 
Евгений Степанищев / Evgeny Stepanischev
