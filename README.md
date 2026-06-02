# Monster Scraper OOP Inheritance & Polymorphism Visualizer

## 1. Project Purpose

This project visualizes the object-oriented structure of the Python console game `monster_scraper` as an interactive web page.

The main purpose is to show inheritance and polymorphism from the original Python OOP design. Users can click class cards and see how different subclasses override and execute the same `attack(target)` method in different ways.

## 2. Original Python Code Structure

The original game is based on the following classes:

- `CharacterADT`: abstract class that defines common character behavior
- `Character`: base character class with HP, attack power, damage, healing, and alive checks
- `Player`: player class with inventory, weapon, scrap, and custom attack behavior
- `NormalMonster`: monster class with reward `10` and custom attack behavior
- `EliteMonster`: stronger monster class with reward `20` and custom attack behavior
- `BossMonster`: boss monster class with reward `35` and custom attack behavior
- `TrainingDummy`: practice target class with custom attack and damage behavior
- `Item`: base item class
- `Weapon`: item subclass with bonus attack
- `HealingItem`: item subclass with healing amount
- `Game`: class that manages the player, monsters, items, battles, safe zone, and shop flow

## 3. Inheritance Structure

Character hierarchy:

```text
CharacterADT -> Character -> Player
CharacterADT -> Character -> NormalMonster
CharacterADT -> Character -> EliteMonster
CharacterADT -> Character -> BossMonster
CharacterADT -> Character -> TrainingDummy
```

Item hierarchy:

```text
Item -> Weapon
Item -> HealingItem
```

## 4. Polymorphism

The web app calls the same method, `attack(target)`, on different objects.

However, each object has its own overridden version of `attack(target)`, so the result changes depending on the actual class type:

- `Player.attack(target)`
- `NormalMonster.attack(target)`
- `EliteMonster.attack(target)`
- `BossMonster.attack(target)`
- `TrainingDummy.attack(target)`

This demonstrates polymorphism because one common method call produces different behavior at runtime.

## 5. Technologies Used

- HTML5
- Tailwind CSS CDN
- Vanilla JavaScript

## 6. How to Run

Open `index.html` in a web browser.

No backend server or Python execution is required.

## 7. Deployment Information

GitHub Repository URL:

```text
https://github.com/mrkai1228/CS-Assignment-2
```

Vercel URL:

```text
Paste Vercel deployment URL here
```
