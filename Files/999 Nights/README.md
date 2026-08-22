# 999 Nights — Treasure & Landmark Coordinates

Coordinate lists for the **999 Nights** roguelite map (Warren Continent), extracted from the shipped game data.

## Regions

| ID | Region |
|----|--------|
| 001 | Chocolate Volcano |
| 002 | Milk Ice Mountain |
| 003 | Amber Syrup Lake |
| 004 | Crimson Castle |
| 005 | Camp |
| 006 | Fuzzy Village |

The six regions occupy completely separate parts of the world grid, so a coordinate alone identifies its region unambiguously.

## Files

| File | Count | What it is |
|------|-------|------------|
| `Common Chest.txt` | 111 | Common Chest — the base loot tier |
| `Valuable Chest.txt` | 59 | Valuable Chest — the middle loot tier |
| `Rare Chest.txt` | 50 | Rare Chest — the top loot tier |
| `Mysterious Chest.txt` | 30 | Mysterious Chest — roll the dice to decide the reward |
| `Trap Chest.txt` | 10 | Bait chest that locks the room and spawns enemies |
| `Bonfire.txt` | 48 | Bonfire — rest, identify and salvage equipment, Warehouse access, fast-travel target, respawn point after a defeat |
| `Golden Pig Hiding Spot.txt` | 54 | Spots the Puffyhog bolts to during the catch event |

**260 chests in total.**

## Line format

```
Region name, X, Y, Z
```

Sections are grouped by region and each header carries its own count:

```
===== [Region 001] Chocolate Volcano (22) =====
```

Coordinates are world-space UE units (1 unit = 1 cm), written at single-precision accuracy — the same values the game itself uses.

## Chests per region

| Region | Common | Valuable | Rare | Mysterious | Trap | Total |
|--------|-------:|---------:|-----:|-----------:|-----:|------:|
| Chocolate Volcano | 22 | 14 | 14 | 7 | 1 | 58 |
| Milk Ice Mountain | 33 | 10 | 12 | 7 | 0 | 62 |
| Amber Syrup Lake | 18 | 14 | 8 | 7 | 3 | 50 |
| Crimson Castle | 18 | 14 | 15 | 7 | 6 | 60 |
| Camp | 13 | 3 | 1 | 0 | 0 | 17 |
| Fuzzy Village | 7 | 4 | 0 | 2 | 0 | 13 |

Every region except Camp and Fuzzy Village clears the "open 10 chests in this region" objective several times over.

## What to expect

- **Tiers.** Common to Valuable to Rare is the loot ladder. Rare chests are the ones worth a detour; Crimson Castle carries the most of them (15), Chocolate Volcano is next (14).
- **Mysterious Chest.** Roll the dice to decide the reward. Seven per region in Volcano, Snow, Lake and Castle; only two in Fuzzy Village; none at Camp.
- **Trap Chest.** Opening it seals the area and spawns a wave. Six of the ten sit inside Crimson Castle, so treat unattended chests there with suspicion.
- **Bonfires** are the hub of a run: rest, identify and salvage gear, reach the Warehouse, and respawn there after a defeat. Once lit, a bonfire also becomes a fast-travel target on the map, so lighting them early pays off. Milk Ice Mountain, Chocolate Volcano and Amber Syrup Lake are well covered; Fuzzy Village has none.
- **Camp and Fuzzy Village** are hub areas rather than runs. Their chests are static scenery pickups, not part of a region clear.
- **Golden Pig Hiding Spot** lists where the Puffyhog runs to during the catch event, not where it starts. They cluster in tight groups, so knowing one spot usually tells you where the next two are.

## Caveats

- Positions are the placed world positions. Whether a chest is *present* in a given run still depends on region, round and difficulty state — a listed coordinate is a place a chest can be, not a guarantee for every run.
- Round variants (the same spot re-used across later rounds) are listed once.
- Chest counts here are placements in the map data, which is why they run higher than what a single run through a region will show you.