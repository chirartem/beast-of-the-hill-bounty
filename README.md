# Beast of the Hill + Bounty

StarCraft II extension mod: a king-of-the-hill free-for-all with a bounty for kills. It works on any melee map: pick it as the extension mod in a custom game lobby.

*Русская версия ниже.*

## How it plays

- A red circle is placed as close to the map centre as possible.
- Whoever holds the circle alone when the round timer runs out scores a point. The first to reach the points-to-win setting wins, and allies win together.
- If several players are on the circle when the timer ends, the round goes into overtime ("The point is contested!") until only one player remains.
- Priorities on the circle: ground > cloaked or burrowed ground > air > cloaked air > temporary units > eggs and cocoons. Buildings and hallucinations never count.
- While you hold the circle alone you gain minerals every second. In a team the income is split evenly between all teammates; a leftover mineral goes to a different teammate each second (5 for two players: 3 + 2, then 2 + 3).
- Bounty: killing an enemy unit gives you a share of its cost (minerals and gas). Buildings, hallucinations and your own units give nothing.
- The circle cannot be built on: its cells show red in the placement grid.

## Lobby options

| Option | Values |
| --- | --- |
| Bounty (%) | 0–100 in steps of 10 |
| Round 1 / Round 2 / Round 3+ time (min) | 1–5 |
| Points to win | 1–5 |
| Zone minerals (per sec) | 5, 10, 15, 20, 25 |
| Zone visibility | Always visible / Hidden (the circle itself is always visible) |
| Starting workers | 8 (current) / 12 (classic, with classic town-hall supply) |

## Interface

- Top right: round timer, score table (sorted by points, in player colours), and "S" and "?" buttons for players.
- Observers see the timer, the score and a bounty table (how much each player earned from kills). They do not get the buttons.
- Countdown warnings at 2 min, 1 min, 30, 20, 10 and 5 s, with a minimap ping, plus a chat message for each round result.
- Players who leave the game are removed from the tables.

## Circle placement

- The mod picks the nearest spot to the centre that is flat, walkable, on one cliff level, not in hiding grass, and free of minerals, geysers and player buildings.
- Neutral objects in the way (Xel'Naga towers, rocks, critters) are removed.
- Map fog, mist and steam decorations that cover the circle are removed. Effects created by units and abilities are never touched.

## Repository layout

- `src/Beast of the hill + bounty.SC2Mod/` is the mod unpacked into its component files, so changes are easy to read. The StarCraft II Editor can open this folder directly.
- `src/.../Base.SC2Data/Lib439EC7DD.galaxy` is the generated trigger library, including the hand-written "BountyHUD" script (HUD, rounds, circle placement, bounty table, observers).
- `release/Beast of the hill + bounty.SC2Mod` is the packed mod file, ready to use.

To try it locally, put the `.SC2Mod` file in your `StarCraft II/Mods` folder, add it as a dependency of a test map in the editor, and run the test (Ctrl+F9). Published versions are available in-game on the EU and US servers under the name "Beast of the hill + bounty".

---

# Beast of the Hill + Bounty (RU)

Мод расширения для StarCraft II: «Царь горы» для всех против всех с наградой за убийства. Работает на любой карте. Выберите его как модуль расширения в лобби своей игры.

## Как играть

- Красный круг появляется как можно ближе к центру карты.
- Кто один стоит на круге, когда заканчивается таймер раунда, получает очко. Побеждает тот, кто первым наберёт нужное число очков. Союзники побеждают вместе.
- Если на круге несколько игроков, раунд продолжается («The point is contested!»), пока не останется один.
- Приоритеты на круге: наземные > невидимые или закопанные наземные > воздушные > невидимые воздушные > временные юниты > яйца и коконы. Здания и галлюцинации не учитываются.
- Пока вы один на круге, вы каждую секунду получаете минералы. В команде доход делится поровну между всеми союзниками; лишний минерал каждую секунду достаётся другому игроку (5 на двоих: 3 + 2, потом 2 + 3).
- Награда: за убийство вражеского юнита вы получаете часть его стоимости (минералы и газ). За здания, галлюцинации и своих юнитов награды нет.
- На круге нельзя строить: его клетки при постройке показаны красными.

## Настройки лобби

| Настройка | Значения |
| --- | --- |
| Bounty (%) | 0–100 с шагом 10 |
| Время 1-го, 2-го и 3+ раунда (мин) | 1–5 |
| Points to win | 1–5 |
| Zone minerals (per sec) | 5, 10, 15, 20, 25 |
| Zone visibility | Always visible / Hidden (сам круг виден всегда) |
| Starting workers | 8 (текущий патч) / 12 (классика, с прежним снабжением от главных зданий) |

## Интерфейс

- Справа вверху: таймер раунда, таблица очков (по убыванию, цветами игроков) и кнопки «S» и «?» для игроков.
- Обсерверы видят таймер, очки и таблицу наград (сколько каждый игрок заработал на убийствах). Кнопок у них нет.
- Предупреждения за 2 мин, 1 мин, 30, 20, 10 и 5 секунд, отметка на мини-карте и сообщение в чате об итоге раунда.
- Вышедшие из игры игроки убираются из таблиц.

## Где появляется круг

- Мод ищет ближайшее к центру место: ровное, проходимое, на одном уровне высоты, не в траве-укрытии, без минералов, газа и зданий игроков.
- Мешающие нейтральные объекты (башни Зел'Нага, камни, животные) удаляются.
- Туман, дымка и пар с карты, закрывающие круг, убираются. Эффекты юнитов и способностей не трогаются.

## Файлы

- `src/Beast of the hill + bounty.SC2Mod/`: мод, распакованный по отдельным файлам. Редактор StarCraft II открывает эту папку напрямую.
- `release/Beast of the hill + bounty.SC2Mod`: готовый файл мода.
