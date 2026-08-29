# 999 Nights — Treasure & Landmark Coordinates

Coordinate data for the **999 Nights** roguelite map on Warren Continent

## Regions

| ID | Region |
| --- | --- |
| 001 | Chocolate Volcano |
| 002 | Milk Ice Mountain |
| 003 | Amber Syrup Lake |
| 004 | Crimson Castle |
| 005 | Camp |
| 006 | Fuzzy Village |

Each region occupies a separate part of the world grid, so coordinates can be identified by region without overlap

## Files

| File | Count | Contents |
| --- | ---: | --- |
| `Common Chest.txt` | 111 | Common chest locations |
| `Valuable Chest.txt` | 59 | Valuable chest locations |
| `Rare Chest.txt` | 50 | Rare chest locations |
| `Mysterious Chest.txt` | 30 | Mysterious chest locations |
| `Trap Chest.txt` | 10 | Trap chest locations |
| `bonfire.txt` | 48 | Bonfire locations |
| `Golden Pig Hiding Spot.txt` | 54 | Puffyhog hiding locations |

**Total chest locations: 260**

## Chest Count by Region

| Region | Common | Valuable | Rare | Mysterious | Trap | Total |
| --- | ---: | ---: | ---: | ---: | ---: | ---: |
| Chocolate Volcano | 22 | 14 | 14 | 7 | 1 | 58 |
| Milk Ice Mountain | 33 | 10 | 12 | 7 | 0 | 62 |
| Amber Syrup Lake | 18 | 14 | 8 | 7 | 3 | 50 |
| Crimson Castle | 18 | 14 | 15 | 7 | 6 | 60 |
| Camp | 13 | 3 | 1 | 0 | 0 | 17 |
| Fuzzy Village | 7 | 4 | 0 | 2 | 0 | 13 |

## Chest Types

- **Common Chest** — base loot tier
- **Valuable Chest** — middle loot tier
- **Rare Chest** — highest regular loot tier
- **Mysterious Chest** — reward is decided when opened
- **Trap Chest** — opening it seals the area and spawns enemies

Crimson Castle has the most Rare Chests with **15**, followed by Chocolate Volcano with **14**

## Bonfires

Bonfires can be used for rest, equipment management, Warehouse access, respawning, and fast travel after activation

Milk Ice Mountain, Chocolate Volcano, and Amber Syrup Lake have multiple bonfire locations while Fuzzy Village has none

## Golden Pig Hiding Spots

`Golden Pig Hiding Spot.txt` contains locations the Puffyhog can run to during the catch event

These are hiding locations rather than starting positions

## Notes

- A listed coordinate is a possible spawn location and does not guarantee the chest will appear in every run
- Chest availability can vary by region, round, and difficulty state
- Reused locations across round variants are listed once
- Camp and Fuzzy Village function more like hub areas than standard run regions
