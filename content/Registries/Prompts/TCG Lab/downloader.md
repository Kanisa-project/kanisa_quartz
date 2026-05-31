Downloading will fetch cards from the WEB2 API and attempt to download the image while also adding it to the local database. Other [[tcg_lab#LABs|LABs]] will then be able to pull from the local database to perform the LABs duties.

Downloader profiles can contain `card_criteria` or `specific_card` keys, each needing different fields to be filled in.

### card_criteria
Using the `card_criteria` key will result in multiple cards that match the values of the selected profile. Only one needs to be filled in

| Key/field name | Description                                          |
| :------------: | ---------------------------------------------------- |
|      name      | Whole or part of a name of the cards being searched. |
|     rarity     | Rarity of the cards to appear in the results.        |
|     color      | The color for the cards to be found.                 |
|     artist     | The name of the artist that designed the cards.      |
|      type      | The type of cards to match in finding.               |
|      set       | Which released set to find cards from.               |


### specific_card
The `specific_card` key returns a single card based on the `set` and `card_number` provided in the profile that's selected. Both are required to find the correct card.

| Key name    | Description                                 |
| ----------- | ------------------------------------------- |
| set         | The set in which the card was released in.  |
| card_number | The number of card in position for the set. |
