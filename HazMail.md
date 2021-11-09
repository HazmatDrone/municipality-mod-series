#### Dependencies: none
Comprehensive mail system.
## Mailboxes
- Allow mail to be sent to them, have an inventory of 27 slots
- Mail cannot be sent if all 27 slots are filled
## Mail
- Letters and stamps can be crafted.
- Letters contain four main parts: a recipent, a body, an inventory, and stamps.
- The recipent is a mailbox (not a player), which can be selected from a list (with search by mailbox name or player name)
- The message body accepts text to accompany the letter
- The inventory accepts up to 9 stacks of items. Each stack or two will change the appearance, starting with an envelope for no items, to a small parcel for one or two stacks, to a large box for all 9 stacks.
- The stamp cost is one stamp for the message plus one stamp for each stack
-  Each mailbox is given a name and will display either the player or [[HazOrgs]] entity connected to it

## Post boxes
- Clicking on post boxes with mail will send the mail, or else show an error explaining why the mail cannot be sent.
- The letter is sealed when it is sent - the contents can't be accessed without ripping it open and the message is permanent. Contents can't be added back to a letter either.

## Delivery
### Automatic
- By default, you can craft 4 stamps with 1 paper and 1 ender pearl
- The mail by default will instantly teleport to the inventory of the mailbox.

### Manual
- Mail can be delivered manually by players instead. In this case, stamps don't require ender pearls, but instead can be minted by a postman or [[HazOrgs]] entity with the purpose of being sold. 