# Shoplifting

Some shops carry goods you can take without paying. Picking one up starts a short interaction where the staff may or may not notice you. Getting caught costs you the item, gets you refused service, and can end with the shop calling the Security Office.

## Stores with stealable goods

`Shoplifting Store.txt` lists 20 store locations across four districts.

| Store | Locations | Goods |
|---|---:|---|
| 2-Four Convenience Store | 4 | Refreshing Fruity, Refreshing Glacier, Gubichi Original Flavor Chips, Gubichi Cucumber Flavor Chips, Crave Bites! Milk Flavor, Crave Bites! Chocolate Flavor |
| Alice's Bakery | 4 | Bread |
| Bamboo Pharmacy | 4 | Cooly Cool Refresher, Purification Guard Lozenges, Blink! Wink Battle!, Great Defender!, Zhu! Vitamin! |
| DSD POP | 3 | Asahi Inori - Cobalt |
| Akratos - Coffee Bean Shop | 3 | 9°C Coffee Beans |
| Puka Candy | 2 | Chocolate |

Bridge Crossings has 5 of these stores, Illusion Town 3, Miguel District 7, New Herland District 5. Unheard Shores, Duskmoor and Sunni Island have none.

Fresh food stalls also carry stealable goods, but they are not named in the store list:

| Goods | Pickups |
|---|---:|
| Lake Fish, Sea Fish | 8 |
| Fruit | 4 |
| Vegetables | 4 |
| Meat | 4 |

## Goods pickup points

The individual items sit at fixed points inside the shops. They are in `..\Random Item.txt` under the name `Steal Goods`.

| Area | Points |
|---|---:|
| Bridge Crossings | 19 |
| Illusion Town | 15 |
| Miguel District | 28 |
| New Herland District | 29 |
| **Total** | **91** |

## Making the attempt

Interacting with an item gives you a choice of how to handle it. The staff watches while you decide.

Taking it:

- Slip it into your pocket
- Take it as if nothing happened
- Take it calmly
- Take it hesitantly
- Take it nervously

Backing out:

- Decisively put it back where it was
- Hesitantly put it back where it was
- Reluctantly put it back where it was

There are also options that do not steal anything but disturb the shop: give it a firm squeeze, unwrap it, drop it accidentally, bump into the shelves accidentally, sweep the item off the shelf, knock over the shelves.

The calmer choices draw less attention. Hesitating gives the staff a chance to spot you first.

## Getting caught

If the staff notices, they call you out and ask for the item back or ask you to pay. Paying settles it and you keep the goods. Refusing gets you thrown out, and the store stops serving you afterwards. Push it further and they threaten to call the Security Office.

Staff will sometimes let you off instead. They may write it off if they decide you simply forgot your money, or if they believe you were robbed yourself.

## Detention Facility

The Detention Facility has its own version of this. Instead of shelves you steal a spoon from the canteen, and instead of a choice of grabs you wait for the right moment while the people around you look away. Pull it too early and you are spotted.