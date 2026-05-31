   
> [!NOTE] Title
> The registries of a Texioty make up the repository for other Texioty environments to pull from

   
   
   A registry contains multiple different things of a similar nature. It allows for better organizing what a specific [[Texioty/Texioty]] environment can do. These are the first six and will come stock with Texioty:

 - [[command_registry]]
 - [[helper_registry]]
 - [[widget_registry]]
 - [[gaim_registry]]
 - [[prompt_registry]]
 - [[api_registry]]
## Command Registry
 The command registry holds all available commands between each of the helpers and widgets. It activates and deactivates commands based on which mode is currently active. It belongs in the [[Texioty/Texioty]] instance.

## Helper Registry
 The helper registry holds any available [[TexHelpers]] downloaded or built on the computer. Commands should be stored in each helper separately and as the helper is being initialized the commands are registered. It belongs in the [[Texioty/Texioty]] instance.

## Widget Registry
 The widget registry holds the GUI additions. [[Widgets]] are built from [[TexHelpers]] and allow for graphical advantages like images and animations. Not all helpers are widgets, but all widgets are helpers. This may be an unnecessary registry, as it could just be the helper_registry and helpers would have a widget flag to mark it as GUI.
 
## Prompt Registry
 [[BasePrompt|Promptaires]] keep the flow of texioty and ask questions/await responses.

## Gaim Registry
 Gaims are the fun part of texioty. It's essentially a promptaire on a repeated loop, so this may also be unnecessary, as a prompt can just have a gaim flag to mark for looping.
 
## API Registry
 Registers and keeps track of different API for calling to the internet/[[kNet]]


