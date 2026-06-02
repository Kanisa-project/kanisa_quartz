

> [!NOTE] Title
> The registries of a Texioty make up the repository for other Texioty environments to pull from.

   
   
   A registry contains multiple different things of a similar nature. It allows for better organizing what a specific [[Texioty]] environment can do. These are the first six and will come stock with Texioty:

 - [[command_registry]]
 - [[helper_registry]]
 - [[widget_registry]]
 - [[gaim_registry]]
 - [[prompt_registry]]

## Command Registry
The command registry holds all available commands between each of the prompters and widgets. It activates and deactivates commands based on which mode is currently active.

## Helper Registry
The helper registry is the basis of [[#Prompt Registry]] and [[#Widget Registry]], seeing as they are both [[TexHelpers]].
 
### Prompt Registry
The prompt registry holds the TUI additions. [[Prompts|Promptaires]] keep the flow of texioty and ask questions/await responses. Any helper that asks multiple questions and can perform many tasks but doesn't have a GUI element, belongs in this registry.

### Widget Registry
 The widget registry holds the GUI additions. [[BaseWidget|Widgets]] allow for graphical advantages like images, animations, buttons, sliders and a lot of other options. If a helper has anything more than text, it belongs in this registry.
 
## Gaim Registry
 Gaims are the fun part of texioty, they can be TUI, GUI or both.                          
 
## API Registry
 Registers and keeps track of different API for calling to the internet/[[kNet]]


