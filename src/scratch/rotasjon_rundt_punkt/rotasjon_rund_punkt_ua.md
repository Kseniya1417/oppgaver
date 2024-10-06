---
title: 'Обертання навколо точки'
level: 1
author: 'Карл А. Мірланд'
language: ua
---


# Вступ {.intro}

У цьому завданні ми імпортуємо геометричну фігуру і потім будемо її
`обертати`{.blockmotion} УВАГА! Якщо ви вже виконали завдання з обертання навколо
власної осі, ви можете пропустити Крок 1 і просто завантажити ваше
попереднє завдання з папки "Мої проєкти"

![Зображення капелюху чарівника](../rotasjon/Geometri.png)


# Крок 1: Підготовка {.activity}

*Щоб було простіше почати, ми візьмемо готову фігуру з бібліотеки
Scratch. Ця фігура схожа на рівнобедрений трикутник.*

## Контрольний список {.check}

- [ ] Почніть новий проєкт.

- [ ] Видаліть фігуру кота, клацнувши на неї правою кнопкою миші та обравши `видалити`.

- [ ] Додайте нову фігуру. Натисніть на кнопку "Обрати персонаж” ![Velg figur fra
      biblioteket](../bilder/hent-fra-bibliotek.png)-knappen og velg
      trollmannshatten. Vi har brukt `Ting/Wizard Hat`-figuren.

- [ ] Назвіть нову фігуру `Чарівний капелюх`.

- [ ] Перш ніж розпочати основне завдання, ми додамо маленьку
допоміжну функцію на випадок, якщо станеться щось несподіване:


  ```blocks
  коли [клавішу n v] натиснуто
  показати
  повернути у напрямку [90 v]
  перемістити в x: (0) y: (0)
  ```

- [ ] Якщо зараз станеться щось несподіване, потрібно лише
натиснути клавішу "N" на клавіатурі, і  `Чарівний капелюх`
повернеться на вихідну позицію, щоб ви могли спробувати
знову.

## Тестування проекту {.flag}

- [ ] Використовуйте вказівник миші, щоб перемістити `Чарівний капелюх` в інше місце на зображенні.

- [ ] Натисніть "N" на клавіатурі. Чи повертається `Чарівний капелюх`
в центр зображення? Якщо так: переходьте до кроку 2. Якщо
ні: перевірте, чи встановлено англійську мову на клавіатурі.
Також перевірте та виправте код, а тоді натисніть "N" на
клавіатурі ще раз.


# Крок 2: Обертання в системі координат {.activity}

- [ ] Імпортуйте фон "xy-grid", натиснувши на кнопку “Обрати тло”.

- [ ] Виберіть `Чарівний капелюх` у скрипті

  ```blocks
  коли [клавішу n v] натиснуто
  показати
  повернути у напрямку [90 v]
  перемістити в x: (0) y: (0)
  ```

  змініть значення x на -100, а значення y на 100.

- [ ] Зверніть увагу на точку, де перетинаються осі x (горизонтальна)
і y (вертикальна). Ця точка називається початок координат і є
точкою, де x = 0 і y = 0.

## Тестування проекту {.flag}

- [ ] Натисніть "N" на клавіатурі. `Чарівний капелюх` повинен
опинитися точно в точці перетину сірих ліній для X = -100 і Y = 100.

- [ ] Якщо все виглядає правильно, переходьте до наступного кроку.

- [ ] Якщо щось виглядає неправильно, спробуйте знайти помилку
в коді а тоді натисніть "N" ще раз.


# Крок 3: Чарівний капелюх обертається навколо початку кординат {.activity}

Тепер ми будемо обертати `Чарівний капелюх` навколо початку координат простим способом.

- [ ] Створіть цей скрипт для `Чарівний капелюх`:

  ```blocks
  коли клавішу [стрілка праворуч v] натиснуто
  перемістити на (200) кроків
  поворот @turnRight на (90) градусів
  ```

## Test prosjektet {.flag}

- [ ] Trykk tasten "pil høyre" på tastaturet. Hva skjer? Fortsett til Hattulf er
      tilbake ved startpunktet sitt.

- [ ] Hvis du studerer koden vi nettopp laget til Hattulf, ser du at vi ber
      Hattulf gå 200 steg. Hvorfor må vi gå så langt?

- [ ] Prøv å endre på antall steg Hattulf tar. Ender Hattulf opp på samme sted
      som han startet etter at du har trykket "pil høyre" fire ganger?


# Steg 4: En ny venn! {.activity}

- [ ] Legg til en ny figur. Denne gangen skal du få velge figur selv. Hvis den
      blir veldig stor i forhold til alt det andre, kan du krympe den ned til en
      passelig størrelse. Kall den nye figuren for "Venn"

- [ ] Lag en kopi av "Når N trykkes"-skriptet fra Hattulf til Venn, men endre
      y-verdien til 50.

- [ ] Kopier også over "Når pil høyre trykkes"-skriptet fra Hattulf, men halver
      både antall steg og antall grader i skriptet.

- [ ] For litt mer moro kan du legge til en linje med kode som skrur på
      `pennen`{.blockpen} for begge figurene. Øverste del av pil høyre-skriptet
      skal da se slik ut:

  ```blocks
  når [pil høyre v] trykkes
  penn på
  ```

## Test prosjektet {.flag}

- [ ] Trykk pil høyre. Hva skjer?

- [ ] Trykk pil høyre slik at Hattulf kommer tilbake til utgangspunktet. Hvor
      langt har Venn kommet nå?

- [ ] Hvor mange ganger på du trykke for at Venn kommer tilbake til
      utgangspunktet?

- [ ] Klarer du å justere utgangspunktet til Venn, slik at figuren har like lang
      avstand til origo for hver gang du trykker pil høyre?
