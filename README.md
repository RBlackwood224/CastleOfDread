# Castle of Dread

A browser-based text-adventure roguelite. Cross the Lava Bridge, explore a 50-room cursed castle whose contents are different every run, and find out who really controls the dragon, and what became of Princess Lysandra.

No installation, no build step, no dependencies: plain HTML, CSS and JavaScript.

## Play

- **Locally:** download or clone the repo and open `index.html` in any modern browser.
- **On GitHub Pages:** *Settings → Pages → Deploy from branch → `main` / root*. The game will be served at your Pages URL.

Progress is stored in your browser's `localStorage` only. Nothing is sent anywhere.

## Features

- **50 rooms, a different castle every run:** the layout is fixed, but shops, traders, chests, mimics, dark rooms, riddle spirits and enemies are randomized per run.
- **3 classes:**

  | Class | Style |
  |---|---|
  | Warrior | High attack and carry weight, straightforward melee |
  | Wizard | Mana-driven spells, tomes and staves, faster levelling |
  | Rogue | Best flee chance, daggers and bows |

- **Zones & enemy pools:** danger scales with how deep you are. The Lower Halls, Cellars, Garden, Upper Manor and Tower Approach each favour different creatures. About 20 enemy types, each with their own behaviour (lifesteal, poison, shrieks that shake your aim, charged heavy blows, packs on higher difficulties).
- **Castle Mood (Dread):** the castle reacts to reckless play and close calls, and grows more dangerous until things calm down.
- **Echoes:** you sometimes hear something coming, but stone lies about direction.
- **Respawns:** cleared rooms don't stay empty forever.
- **Poison & status effects:** poison burns for a couple of rooms or can be cured instantly with an Antidote. Also Rattled, Shaken, Last Stand and flee fatigue.
- **Economy & crafting:** Blacksmith (weapons, whetstones, Tempered Ore upgrades) and Alchemist (potions, ingredients, recipes), plus herb/mushroom crafting. Meeting a merchant gives you a summoning scroll, but summoned prices run higher.
- **Chests with tools:** trapped, stuck or biting chests need the right tool (Lockpick, Crowbar, Oil Can, Bucket of Water).
- **Cursed items & riddles:** powerful gear with hidden prices, and spirits that won't let you pass until you answer.
- **Level-up choices:** each level you pick where the point goes (HP, Attack, Defense, Mana, Carry Weight, Luck or Flee).
- **Limited saving:** one free save per run, plus rare Save Scrolls hidden in the castle.
- **Bestiary & endings:** creatures seen and endings found persist across runs.
- **4 difficulties:** Easy, Normal, Hard and Extreme (stronger enemies, faster Dread, multi-creature encounters). Changeable any time in Settings.
- **In-game Manual** (menu or `manual` command), and a map that reveals as you explore.

## Commands

| Command | What it does |
|---|---|
| `go north/south/east/west` | Move |
| `attack`, `use <item>`, `equip <item>`, `flee` | Combat and items |
| `inventory` (`inv`), `status`, `map` | Check yourself and the map |
| `take`, `open`, `store` / `retrieve` | Loot, chests and your stash |
| `shop`, `buy`, `sell`, `upgrade`, `craft`, `recipes`, `exit shop` | Merchants and crafting |
| `levelup <stat>` | Spend a level-up point |
| `save`, `load`, `reset` | Save (uses your free save or a Save Scroll), load, restart |
| `bestiary` (or `codex`) | Creatures and endings seen so far |
| `manual` | Full rules |
| `help` | Quick command reference |

## Project structure

```
index.html   page and screens (menu, character creation, story, manual, settings, game)
style.css    styling
script.js    all game logic
images/      menu background
```

## Notes

- English only for now.
- Balance target (bot-simulated win rates, roughly): Easy ~40-60%, Normal ~25-35%, Hard ~15%, Extreme ~5-10%. Wizard is currently the weakest class.

## Credits

Menu background image generated with Google AI.

## License

All rights reserved, unless a license file says otherwise.
