# Pink Paws Heist — Coordinate Data

Coordinate data for **Pink Paws Heist** covering **2,109 loot slots** across the bank

## Contents

| Path | Contents |
| --- | --- |
| `Quick.txt` | Exits, boss positions, and high-value loot clusters |
| `Index/` | Loot item coordinates grouped by item |
| `keycard/` | Keycard coordinates grouped by card |

## Spawn Data

The coordinates represent locations where an item **can** appear

They are not guaranteed spawns, because each slot selects an item from its own loot table during a run

> `Eternal Heart.txt` contains 697 entries, but this does not mean 697 Eternal Hearts appear in one run

## Expected Value

Expected Value or **EV** estimates the average Fons value of opening a loot slot

```text
EV = SUM(weight * value) / SUM(weight)
```

### Example — 3F Gem Safes

| Item | Value | Weight | Chance | EV Share |
| --- | ---: | ---: | ---: | ---: |
| Gold Bar | 1,000 | 858,378 | 85.84% | 858 |
| Smoky Amethyst | 9,999 | 108,940 | 10.89% | 1,089 |
| Lustrous Jade | 88,888 | 27,235 | 2.72% | 2,421 |
| Eternal Heart | 666,666 | 5,447 | 0.54% | 3,631 |
| **Total** |  | **1,000,000** | **100.00%** | **7,999** |

A gem safe is worth roughly **8,000 Fons per open** on average

The Eternal Heart roll is only **0.54%**, but contributes nearly half of the total EV

## Quick.txt

`Quick.txt` contains the most useful locations for fast reference

| Section | Entries | Contents |
| --- | ---: | --- |
| `[Extraction]` | 11 | Extraction doors |
| `[Boss]` | 3 | Boss spawn positions |
| `[Loot Cluster]` | 31 | High-value loot areas |

### Extraction Doors

- 1F — 4
- 2F — 4
- 3F — 2
- 4F — 1

`Exit 4F-001` is located past the final boss room

### Top 5 Loot Clusters

| EV | Slots | Floor | Position | Note |
| ---: | ---: | --- | --- | --- |
| 94,798 | 14 | 3F | -28988.9, 50788.6, 4140.6 | |
| 52,199 | 7 | 3F | -40207.5, 50610.2, 4167.2 | |
| 50,057 | 12 | 3F | -36807.8, 52355.4, 4043.1 | |
| 40,000 | 1 | 2F | -34920.0, 39820.0, 4150.0 | Highest-value single slot |
| 31,250 | 9 | 3F | -32512.7, 52597.5, 4059.9 | |

Four of the top five clusters are on the **3F vault floor**

## Loot Index

Files in `Index/` are separated by loot item and sorted below by value

| File | Rarity | Value | Slots |
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

**Rarity order:** Epic > Rare > Common > Basic

Fresh Tangerine Soda, VC Vitality Drink, and Cooly Cool Pain Relief can also restore HP, so using one means giving up its sale value

## Keycards

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

Vault Access Card I through X correspond to the ten vault doors on 3F

All ten cards can roll from the same **252 slots**

## Notes

- Pink Paws Heist uses its own local coordinate space, separate from the open world
- Do not mix heist coordinates with open-world coordinates
- **Crimson Gem** is a boss drop, so its entries are boss spawn positions rather than pickup positions
- **Artwork Ancient Castle** drops from enemies, so its entries are enemy spawn positions
- **Paw-Paw Coins** are score rewards rather than lootable map items, so they have no coordinate file
- Fons income can be multiplied during limited-time events
