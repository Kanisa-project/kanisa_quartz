   A friar profile contains various ways of changing colors; adding tints, removing tints, color swapping.

|   Property   | Type  | Example | Explained |
| :----------: | :---: | :-----: | :-------: |
| grease_temp  |  int  |   241   |           |
| basket_depth |  int  |    4    |           |
|  cook_timer  | float |  2.679  |           |


## grease_temp
  The grease temp is what allows simple tints of color, changing the RGB values of the entire image. It needs a number between 0 and 765 for the three channels of 255 maxed-out.

## basket_depth
   Basket depth determines some information for the cook_timer to affect the HSB values.

## cook_timer
   The cook timer is what allows sharper changed colors, modifying the HSB values of the entire image. A float allows for a whole number and a partial number, for some reason it'll be needed.