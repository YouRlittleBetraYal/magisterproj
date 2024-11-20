# magisterproj
# Проєкт на Python: Контролери нечіткої логіки

## Опис
Цей репозиторій містить два окремі нечіткі логічні контролери для роботи з **CoppeliaSim**:

- **FLC-1**: Контролер наведення на ціль.
- **FLC-2**: Контролер оминання перешкод.

Обидва контролери запускаються через файл `main.py`, розташований у відповідних папках.

## Вимоги
- **Python**: 3.8.5
- **IDE**: Visual Studio Code

## Структура проєкту

### FLC-1
Папка для реалізації контролера наведення на ціль:
- **main.py**: Основний файл запуску.
- **FLC-1_fuzzy_logic.py**: Контролер нечіткої логіки.
- **graph.py**: Побудова графіків та візуалізація.
- **fcl-1.ttt**: Файл середовища CoppeliaSim без перешкод для тестування наведення на ціль.

### FLC-2
Папка для реалізації контролера оминання перешкод:
- **main.py**: Основний файл запуску.
- **FLC-2_fuzzy_logic.py**: Контролер нечіткої логіки.
- **graph.py**: Побудова графіків та візуалізація.
- **fcl2-02.ttt**: Файл середовища CoppeliaSim із перешкодами для тестування оминання перешкод.
## Скомпільовані .exe
Прикладаю попередньо скомпіловані файли FLC-1, FLC-2
Працездатність тестувалась на OS Windows 10, що до інших - невідомо
1. Відкрийте файл з середовищем для контролера у потрібній папці (`fcl-1.ttt для FLC-1` або `fcl2-02.ttt для FLC-2`) за допомогою Copeliasim edu
2. Запустіть файл `main.exe` у потрібній папці (`FLC-1` або `FLC-2` відповідно )
   - Папка для контролера **FLC-1**: Наведення на ціль.
   - Папка для контролера **FLC-2**: Оминання перешкод.
3. Для закінченя роботи програми слід нажати Ctrl + C у вікні консолі, тим самим програма зупиниться та побудує графіки (переше ніж змоделює інший графік попередній потрібно закрити)
## Інструкція з запуску без компіляції
1. Встановіть Copeliasim Edu версія для університетів
2. Встановіть python версії 3.8.5
3. Встановіть бібліотеки командами: pip install numpy, pip install matplotlib, pip install coppeliasim-zmqremoteapi-client
4. Відкрийте файл з середовищем для контролера у потрібній папці (`fcl-1.ttt для FLC-1` або `fcl2-02.ttt для FLC-2`) за допомогою Copeliasim edu
5. Відкрийте файл `main.py` у потрібній папці (`FLC-1` або `FLC-2` відповідно ) за допомогою **Visual Studio Code**.
6. Запустіть скрипт, щоб активувати відповідний контролер:
   - Папка для контролера **FLC-1**: Наведення на ціль.
   - Папка для контролера **FLC-2**: Оминання перешкод.
7. Для закінченя роботи програми слід нажати Ctrl + C у вікні консолі, тим самим програма зупиниться та побудує графіки (переше ніж змоделює інший графік попередній потрібно закрити)
## Призначення основних файлів

- `main.py`: Відповідає за підключення до **CoppeliaSim**.
- `FLC-*_fuzzy_logic.py`: Містить реалізацію контролера нечіткої логіки.
- `graph.py`: Генерує графіки для аналізу роботи контролера.
- `fcl.tt`: файл з середовищем.

