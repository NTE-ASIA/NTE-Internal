# Pink Paws Heist - Coordinate Data

Spawn locations for the Pink Paws Heist game mode, covering **2,109 loot slots**
across the whole bank. Everything here is exact - nothing was paced out or
eyeballed in-game.

## Contents

| Path | What it is |
| --- | --- |
| `Quick.txt` | Cheat sheet: exits, boss, high-value clusters (45 entries) |
| `Index/` | 47 loot items, one file each |
| `Keycard/` | 22 keycards, one file each |

## File format

```
Label, X, Y, Z
```

Coordinates are local to the heist map. They are **not** in the open-world
coordinate space - do not mix the two.

Files are split by floor with headers like:

```
===== [Floor 3F] (86) =====
```

Floors are `Lobby` / `1F` / `2F` / `3F`. `Quick.txt` also has a `Boss` section.

## These are not guaranteed spawns

Each line is a slot where that item **can** roll, not a guaranteed pickup.
On any single run each slot rolls exactly one item from its loot table.

> `Eternal Heart.txt` has 697 lines. That does not mean 697 hearts spawn per
> run - it means those 697 slots each have a small chance of rolling one.

## Expected value (EV)

EV is the average Fons you get from opening one slot, computed from the loot table:

```
EV = SUM(weight * value) / SUM(weight)
```

Worked example - the gem safes on 3F (14 slots):

| Item | Value | Weight | Chance | EV share |
| --- | ---: | ---: | ---: | ---: |
| Gold Bar | 1,000 | 858,378 | 85.84% | 858 |
| Smoky Amethyst | 9,999 | 108,940 | 10.89% | 1,089 |
| Lustrous Jade | 88,888 | 27,235 | 2.72% | 2,421 |
| Eternal Heart | 666,666 | 5,447 | 0.54% | 3,631 |
| **Total** | | **1,000,000** | **100.00%** | **7,999** |

So that safe is worth roughly **8,000 Fons per open** on average. Note that the
0.54% Eternal Heart roll supplies nearly half of the whole EV.

## Reading `Quick.txt`

| Section | Contents |
| --- | --- |
| `[Extraction]` (11) | Extraction doors: 1F x4, 2F x4, 3F x2, 4F x1. `Exit 4F-001` is the one past the final boss room. |
| `[Boss]` (3) | Boss spawn positions. |
| `[Loot Cluster]` (31) | High-value areas. |

Cluster labels decode like this:

```
3F Loot EV94798 x14, -28988.89, 50788.574, 4140.589
 |       |       |    \____________________________/
 |       |       |     centre of the cluster
 |       |       number of spawn slots in the cluster
 |       combined EV of the whole cluster, in Fons
 floor
```

Built by taking the 145 slots with EV >= 2,000, grouping anything within 900
units, and keeping clusters worth 4,000+ EV in total.

### Top 5 clusters

| EV | Slots | Floor | Position | |
| ---: | ---: | --- | --- | --- |
| 94,798 | 14 | 3F | -28988.9, 50788.6, 4140.6 | |
| 52,199 | 7 | 3F | -40207.5, 50610.2, 4167.2 | |
| 50,057 | 12 | 3F | -36807.8, 52355.4, 4043.1 | |
| 40,000 | 1 | 2F | -34920.0, 39820.0, 4150.0 | richest single slot |
| 31,250 | 9 | 3F | -32512.7, 52597.5, 4059.9 | |

Four of the top five sit on the 3F vault floor.

## `Index/` - loot items

Sorted by value.

| File | Rarity | Value (Fons) | Slots |
| --- | --- | ---: | ---: |
| Eternal Heart | Epic | 666,666 | 697 |
| Crimson Gem | Epic | 131,400 | 3 |
| Lustrous Jade | Epic | 88,888 | 722 |
| Giovannis Gilded Statue | Epic | 50,000 | 86 |
| Oceanic Dewdrops | Epic | 40,000 | 69 |
| Orrery | Epic | 27,500 | 210 |
| Starshaker | Epic | 20,000 | 101 |
| Blue and White Porcelain Vase | Rare | 15,000 | 133 |
| Snowfall Emerald | Epic | 15,000 | 69 |
| Cooly Cool Pain Relief | Epic | 12,000 | 92 |
| Smoky Amethyst | Rare | 9,999 | 722 |
| Artwork Deep Forest | Rare | 7,500 | 146 |
| Artwork Ancient Castle | Rare | 6,400 | 88 |
| Red Glaze Vase | Rare | 6,400 | 255 |
| Artwork Green Meadows | Rare | 5,200 | 146 |
| Dark Green Vase | Rare | 5,000 | 255 |
| Geometric Decor | Epic | 5,000 | 539 |
| Artwork Still Life | Rare | 4,000 | 146 |
| VC Vitality Drink | Rare | 4,000 | 92 |
| Ink-Stained Jar | Rare | 3,000 | 564 |
| Phonograph | Rare | 2,800 | 141 |
| Jade Cutter | Rare | 2,500 | 101 |
| Ink-Stained Vase | Rare | 2,000 | 564 |
| Golden Crescent | Rare | 1,500 | 69 |
| Navigators Telescope | Rare | 1,500 | 579 |
| Starseeker Telescope | Rare | 1,200 | 287 |
| Fresh Tangerine Soda | Common | 900 | 202 |
| Gold Gilded Basin | Common | 800 | 668 |
| Cubox Technologies Phone | Common | 750 | 682 |
| Blue and White Porcelain Bowl | Common | 720 | 668 |
| Blue Glaze Vase | Common | 640 | 668 |
| Digital Camera | Common | 600 | 682 |
| Gubichi Original Flavor Chips | Common | 600 | 364 |
| Carved Floral Bowl | Common | 560 | 668 |
| Artwork Drinking in Solitary | Common | 500 | 349 |
| Artwork Chasing Fragrance | Common | 400 | 349 |
| Berry Yogurt Shake | Common | 400 | 254 |
| Nacupeda Model | Common | 400 | 343 |
| Artwork Flower Field | Common | 300 | 349 |
| Asahi Inori Figurine | Common | 300 | 343 |
| Danzaburou Doll | Common | 250 | 343 |
| Artwork Deconstruction | Common | 200 | 349 |
| Fluffy Figurine | Common | 180 | 343 |
| Fortune Cat Decor | Common | 100 | 343 |
| Grape Sparkling Water | Basic | 100 | 364 |
| Manga Duke K | Basic | 50 | 342 |
| Manga Magazine | Basic | 30 | 342 |

Rarity tiers, highest first: **Epic > Rare > Common > Basic**

Fresh Tangerine Soda, VC Vitality Drink and Cooly Cool Pain Relief double as HP
restore consumables - using one costs you its sale value.

## `Keycard/`

| File | Slots | Doors |
| --- | ---: | ---: |
| Advanced Clearance Card I | 852 | 1 |
| Collection Floor Pass | 836 | 1 |
| Common Clearance Card | 836 | 2 |
| Meeting Room Access Card | 836 | 1 |
| Recreation Room Access Card | 836 | 1 |
| Vault Pass | 836 | 1 |
| Assistant Manager Office Access Card | 582 | 1 |
| Electrical Room Access Card | 582 | 1 |
| Security Room Access Card | 582 | 1 |
| Temporary Visitor Pass | 536 | 6 |
| Manager Office Access Card | 262 | 1 |
| Manager Storage Room Access Card | 262 | 1 |
| Vault Access Card I | 252 | 1 |
| Vault Access Card II | 252 | 1 |
| Vault Access Card III | 252 | 1 |
| Vault Access Card IV | 252 | 1 |
| Vault Access Card IX | 252 | 1 |
| Vault Access Card V | 252 | 1 |
| Vault Access Card VI | 252 | 1 |
| Vault Access Card VII | 252 | 1 |
| Vault Access Card VIII | 252 | 1 |
| Vault Access Card X | 252 | 1 |

Vault Access Card I through X map one-to-one to the ten vault doors on 3F.
All ten roll from the same 252 slots, so which one you find is luck.

## Notes

- **Crimson Gem** is a boss drop only. The 3 lines in `Index/Crimson Gem.txt`
  are boss spawn positions, not pickup positions.
- **Artwork Ancient Castle** only drops from enemies, so its coordinates are
  those enemy spawn positions.
- **Paw-Paw Coins** are a score reward currency, not a lootable item, so there
  are no coordinates for them.
- Fons income is multiplied during limited-time events.