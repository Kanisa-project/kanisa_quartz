tcg_lab is a promptaire about working with trading card games and the different elements of each game. 


# TCGs
   Any trading card game that has an available API is able to be made into a promptaire. I'm including the 5 major current ones; Magic the Gathering, Pokemon, YuGiOh, Lorcana and Digimon. 

## Card Searching
  [[downloader]] is the primary way of searching for cards to download and add to the local database. You can make a searching profile with [[profile_make#Downloader]]
## Card Results
   When searching for cards, you'll get a result that isn't normalized or standardized, the next step is to make sure it's easily read for use. Each different LAB will need to know what the difference between Lorcana's Ink vs MTG Mana is. A Monster from Yu-Gi-Oh is not the same type of monster from Digimon which is different from a Pokemon monster.

#### single_card
#### card_batch

---

# LABs
Laboratories are different ways of working with a TCG. There are decks to be generated, images depicted from cards, and puzzles made from lore.


|   Laboratory   |                                             Explanation                                             |
| :------------: | :-------------------------------------------------------------------------------------------------: |
| Depictinator{} |            Depicts a new image from the information of a single card or group of cards.             |
| Card%Puzzler(] |          Sets up a puzzler_profile with information from a single card or group of cards.           |
| TC-Blender 690 | Trading Card blender gets aspects from different cards and blends them into a new nonsensical card. |
| Card-0wn1oad3r |           [[Downloader\|Downloads]] a card or group of cards into the systems directory.            |
| RanDexter-2110 |          Generates a simple random deck list based from a [[decksters\|deckster_profile]].          |

#### [[depictinator|Depictinators]]
Create a depiction from a batch of cards. Using information of the cards, a new image will be created with lines, shapes, colors and stuff.

#### [[puzzlers|Puzzlers]]
Create a word puzzle based off the batch of cards being used. You can make a word search from casting costs or a hangman phrase of flavor text.

#### [[tc-blender|TC Blenders]]
This gathers two different cards and slices, splices and blends them together. Planning for mixing TCGs for truly nonsensical cards.

#### [[downloader|Downloader]]
Download a batch of cards from the API for local storage. Can be used in the TC-blender or even foto_worx.

#### [[decksters|Decksters]]
Generate a deck list of cards based on the batch of cards.



## TCG quick info

|         TCG         | Colors | Types |
| :-----------------: | :----: | :---: |
| Magic the Gathering |   6    |   7   |
|       Pokemon       |   10   |   3   |
|       Digimon       |   6    |   3   |
|       YuGiOh        |   7    |   3   |
|       Lorcana       |   6    |   4   |
