# ultimate-marketplace
TODO: Create minimal self-contained marketplace software



## Features
- Individual accounts
- Pages:
    - Home page. Shows categories and sections for random, trending, featured/sponsored.
    - Category page. Shows a list of all items matching a specific category.
    - Account page. Shows all items being sold from a single account. Shows the average account rating. Shows last signed in date.
    - Item page. Shows the item picture, name, price, ratings/reviews, a 'Buy' button, where it's shipping from. Shows statistics on how much was bought and when, and about how fast shipping is.
    - Buy page. Shows items to buy and final price. Allows inputing payment details (and optional shipping details).
    - Orders page. Shows a list of item purchases.
    - Settings page. Shows a list of settings, like email
    - Registration view. A popup when trying to do something that requires an account.
- Accounts should get a notification when an item is purchased.
- Accounts should get a notification when a purchased item status is changed, like 'shipped' and possibly 'delivered'.
- Accounts should be able to directly message a seller. 

### Features v2
- Maybe: Business accounts (allows for multiple individual accounts to sign in to the same business account). But, need to deal a lot with account permissions within the business account too.
- Ability to upload multiple listings using a standard JSON format (yet to be defined)
- Section for 'Services' and 'Physical Goods'. Workaround: Sellers can use the same framework and specify the service.



## Pricing
- Nominal $10/year for sellers to help ensure active/serious listings. And, to help cover some server costs.
    - Pro: Seemingly less competition for sellers. Buyers wouldn't be wasting time
    - Con: With less sellers, then wouldn't be able to brag about the number of sellers
- 1% fee on all transactions to cover server costs and DDOS protection.



## Items JSON format
```
{
    "items": [
        {
            "name": "Thing 1",
            "description": "A good description of Thing 1",
            "priceInUsd": 10.00,
            "availability": 42
        },
        {
            "name": "Thing 2",
            "description": "A good description of Thing 12",
            "priceInUsd": 12.12,
            "availability": 11
        }
    ]
}
```
Note: Currently, pictures are uploaded afterwards.
