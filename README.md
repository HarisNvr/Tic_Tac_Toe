# Игра "Крестики-нолики"

## Описание

Это простая игра "Крестики-нолики" для 2-х игроков, реализованная на языке Python в двух версиях: консольная и графическая. Игроки поочередно размещают свои символы (крестики или нолики) на игровом поле. Цель игры - первым выстроить три своих символа в ряд, столбец или по диагонали. Результаты игры сохраняются в файл results.txt.

## Установка
- Убедитесь, что у вас установлен Python 3.6 или новее
- Склонируйте репозиторий:
```
git clone https://github.com/HarisNvr/Tic_Tac_Toe.git
```
- Перейдите в директорию проекта:
```
cd Tic_Tac_Toe
```
- Создайте и активируйте виртуальное окружение:
```
python -m venv venv
source venv/bin/activate
```
- Если хотите поиграть в графическую версию, то установите зависимости:
```
pip install -r requirements.txt
```

## Использование

**Существует две версии игры - консольная и графическая.**

- При игре в консольную версию, вам нужно будет вручну пропечатывать в консоли позицию вашего хода.
```
python game_console.py
```
```
  1 2 3
1  | | 
  -----
2  | | 
  -----
3  | | 

Ходит X
Введите номер строки: 1
Введите номер столбца: 1

  1 2 3
1 X| | 
  -----
2  | | 
  -----
3  | | 
```

- В графической же версии вам просто нужно кликать мышкой на свободные клетки, чтобы разместить свой символ.
```
python game_graphic.py
```

## Обработка ошибок

- FieldIndexError: возникает, если введенные координаты выходят за пределы игрового поля.
- CellOccupiedError: возникает, если выбранная ячейка уже занята.
- ValueError: возникает, если введены некорректные значения (не числа).
