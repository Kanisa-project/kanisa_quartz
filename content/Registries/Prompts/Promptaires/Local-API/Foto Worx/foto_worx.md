foto_worx is a [[BasePrompt|promptaire]] for taking an image and applying different filters and/or effects to it, then saving new outcomes of iterations. Themed after restaurant equipment, functions can change color, add shapes, move pixels or move pieces of the foto being worked with.

## Equipment
Each piece of equipment specializes in a part of manipulating the image.

#### Flattop - Flatop_XT 2200
Square off some of the image and move it around, slide it or press it. Steam lids and grill weights with spatulas help this profile.

| XT 2200 settings |    Type     |       Example        |                Explained                |
| :--------------: | :---------: | :------------------: | :-------------------------------------: |
|  spatula_slide   |  direction  |     (0.1, 0.82)      |      (x, y)  ⇒    x ≤ 1.0, y ≤ 1.0      |
|   grill_weight   | box_percent | (0.2, 0.2, 0.8, 0.8) | (x¹, y¹, x², y²)  ⇒    x¹ < x², y¹ < y² |
|    steam_lid     |    bool     |        False         |              True or False              |


#### Slicer - S/p/licer R0T8
Slice off a portion of the image and portion it out for easier plating. Maybe it goes to solid color, maybe it needs fried or grilled, point is it gets sliced with this profile type.

|  R0T8 settings  |   Type    |  Example   |           Explained           |
| :-------------: | :-------: | :--------: | :---------------------------: |
|   slice_item    |    str    |  Cheddar   |     length ≤ 32, a-z, A-Z     |
| slice_direction | direction | (0.3, 0.4) | (x, y)  ⇒    x ≤ 1.0, y ≤ 1.0 |
|    thickness    |   float   |    0.75    |     t  ⇒   0.1 ≤ t ≤ 9.9      |
|     amount      |    int    |     3      |       a  ⇒   0 ≤ a ≤ 9        |
| portion_amount  |   float   |    1.4     |    pa  ⇒   0.1 ≤ pa ≤ 9.9     |

#### Friar - Deep-friar 420
The basket is full, but how full? The grease is hot and a little too low, did you set a timer or is it getting burnt?

| deep-420 settings | Type  | Example |        Explained        |
| :---------------: | :---: | :-----: | :---------------------: |
|    grease_temp    |  int  |   452   |  gt  ⇒   1 ≤ gt ≤ 765   |
|   basket_depth    |  int  |    6    |   bd  ⇒   0 ≤ bd ≤ 9    |
|    cook_timer     | float |   2.2   | ct  ⇒   9.9 ≤ ct ≤ 99.9 |

#### Extruder - Pixtruderer V3
Finds certain pixels and stretches them to plenty of different degrees. Twist them, change them, it's a pixtruder.

| V3 settings | Type | Example |       Explained       |
| :---------: | :--: | :-----: | :-------------------: |
| noodle_base | str  |  Flour  | length ≤ 32, a-z, A-Z |
|   length    | int  |    3    |   l  ⇒   0 ≤ l ≤ 9    |
|  thickness  | int  |    6    |   t  ⇒   0 ≤ t ≤ 9    |
|  is_spiral  | bool |  True   |     True or False     |

#### Printer - Tix>Prit C.R.1
Places words on the image. Direction, font, size, color, are examples of profile settings.


| C.R.1 Settings |   Type    |        Example         |                Explained                 |
| :------------: | :-------: | :--------------------: | :--------------------------------------: |
|  ticket_items  | List[str] | [This, list, is, good] | List of strings<br>length ≤ 32, a-z, A-Z |
|  tix_time_in   |   float   |          1.2           |         tti  ⇒   0.1 ≤ tti ≤ tto         |
|  tix_time_out  |   float   |          3.9           |         tto  ⇒   tti ≤ tto ≤ 9.9         |
|  table_number  |    int    |           64           |            x  ⇒   0 ≤ x ≤ 99             |
|  server_name   |    str    |         Helen          |          length ≤ 32, a-z, A-Z           |

## Platement
The final stage before the server takes the image to displaying, pick some images and put them together into a single plate of cool.