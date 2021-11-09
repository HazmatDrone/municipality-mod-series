#### Dependencies: none
- A simple shop block that comes in a few varieties depending on how you want to flavour your shop
- Shops don't have to rely on inventories - you can connect them to inventories via the use of a catalog
- Shops are designed to support both bartering (e.g. with emeralds or any other Minecraft item) as well as [[HazCurrency]]

### Basic Shops
1. **Simple shops / displays** - Can hold a single trade of items intrinsically, or pull from inventories. Stores the resulting cash.
	- Shop display - show items on top of a simple table with a price by them. Designed with simple tileability in mind to create stalls, kiosks, etc.
	- Glass display case - shows off an expensive item in a secure looking glass display case, e.g. for armor, jewellery, etc
2. **Shelves** - Can hold 9 stacks of any item for as many trades as necessary. Can hold cash in the inventory.
	- Store shelf - a simple shelf that shows off all the stacks of items currently for sale. (the currency and irrelevant items won't be displayed)
	- Bakery display case - A glass cabinet for showing off food. A small heat light can be toggled in the UI to make food appear either preheated.
	- Depot - a shelf-like designed with buying in mind rather than selling. Instead of the sold item being displayed, the bought item will be shown. (E.g. a blacksmith might have a depot purchasing ore from miners, which gradually visually fills up with ore purchased)

### Variants of shops (for later consideration)
1. **Vending machines** - A more expensive, 2x1 standalone structure capable of holding 27 stacks of items, and up to 8 trades.
	- Cannot be linked to a shop system via catalog.
	- Can hold cash in the inventory. Can also accomodate for cashless purchases.
	- Can be set to dispense or extract a fluid or power instead of selling items
	- Can be dyed to stand out, and a variety of textures can be selected for the sides to flavour/brand the vending machine.
	- Vending machines require power to operate. By default, this is burnable fuel - each trade will consume 100 units of fuel (1/8th of a piece of coal). If there's Forge Energy on the server, a vending machine can be made to use FE instead.
2. **Meters** - designed with automation in mind, they are linked to two digital accounts. They can transfer items, fluids or power. As items/fluids/energy is transferred, money is automatically deducted based on a rate set by the first account holder. Optionally, a reverse-rate can be charged for items/fluids/energy sent through in reverse.

## Catalog
- The catalog shows all the trades available in the shop as well as the transaction history 
	- A small note can be written under each catalog entry for the purpose of advertising or indicating aisle number, etc etc
- The catalog allows the shopkeeper to remotely interface with every connected shop (except for depositing and withdrawing items), allowing for easy adjustment of prices and other config
- Storage can be defined as input (goods), output (earnings), or both; shops will automatically pull and push items accordingly
- When linking things to the catalog, you can choose between 16 colour frequencies in order to have shops only interact with storage of the same frequency. Storage can have multiple frequencies set.
- A budget can be set for each trade, as to prevent going broke from flooding (e.g. a limit of 64 diamonds can be set). This is set per-unique trade, so 1 diamond for 2 emeralds and 1 diamond for 4 emeralds would be budgeted separately, but two shops doing the same trade would be accounted for together.

## Mail Trading with [[HazMail]]
- If [[HazMail]] is installed, you can create mail trading shops. These will allow you to send mail requests for items, which will then be shipped to a mailbox of your choice.
- If the trade is bartering, you need to attach the required fee (e.g. emeralds) to the mail in order for the trade to go through (post boxes won't let you send an order with an insufficient fee for the order)

## Renting/Purchasing Land with [[HazSecurity]]
If [[HazSecurity]] is installed, there will be a booth for renting and purchasing stakes of land. 
- The security tool will also have a rental/purchase expand region option in the mode list.
- Rental booths allow a player to rent regions to other players. They can set a barter or [[HazCurrency]] price per-hour or per-day, as well as a minimum and maximum stay length. When the booth is placed down, a player can either choose to convert an existing colour region to the rental booth, or to lay it down from scratch. The player does not get full access rights necessarily.
- Purchasing allows a player to permanently sell a region to another player. Upon purchase, the buyer picks a colour for the new region to take up. The player purchasing will gain **full access rights** over the land. 