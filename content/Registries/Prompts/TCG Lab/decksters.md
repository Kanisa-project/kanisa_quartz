   A deck is a pile of cards with planned purpose and hopeful expectations. Sometimes the plan goes left or the hopes get crushed under the weight of defeat. We continue, though. Continue with planning better plans, and lowering expectations to raise a higher hope. It's not the starting point that matters, it's the testing and training you put into a deck that makes it the best it can be.


### Deck Archetypes

| Archetype | Description                                                         |
| :-------: | ------------------------------------------------------------------- |
|   Aggro   | Aggressive cards battling with empowering support cards.            |
| Midrange  | Cards of efficiency, standing the test of time and facing victory.  |
|  Control  | Destructive and controlling cards with enough resources for it all. |
|   Combo   | Cards that hold cards to bounce other cards into winning.           |
|  Engine   | Solid turn plans consistently using cards to your advantage.        |

Each card will get judged and scored by the contents of its being.

|    Card Type     | Benevolent | Malevolent | Board Time |
| :--------------: | :--------: | :--------: | :--------: |
| Creature/Monster | defensive  | offensive  | permanent  |
| Artifacts/Items  |  helpful   |  hurtful   | permanent  |
|  Spells/Actions  |  creative  | destuctive | temporary  |

### Deckster Properties
   All of these properties are required

| Dexr Properties   | Type | Example |                              Explained                              |
| ----------------- | :--: | :-----: | :-----------------------------------------------------------------: |
| number_of_cards   | int  |   60    |                 Number of cards to be in the deck.                  |
| resource_portion  | int  |   25    | Percentage of the deck to be resources like lands, energies or ink. |
| creature_portion  | int  |   25    |         Percentage of the deck to be creatures or monsters.         |
| permanent_portion | int  |   25    |        Percentage of the deck to be non-creature permanents.        |
| temporary_portion | int  |   25    |      Percentage of the deck to be temporary actions or spells.      |
| permanents_split  | dict |  below  |       The split of Malevolent vs Benevolent permanent cards.        |
| temporarys_split  | dict |  below  |       The split of Malevolent vs Benevolent temporary cards.        |

```
"permanents_split": {
    "malevolent_percent": 35,  
    "benevolent_percent": 65  
  }
```

```  
"temporarys_split": {  
    "malevolent_percent": 65,  
    "benevolent_percent": 35  
  }
```