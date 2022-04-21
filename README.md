# rofi-monitor-selector

Simple script using rofi as GUI to setup multi-monitor environment. 

Select outputs and then select action :

![Outputs menu](./assets/output_selector_menu.png) -> 
![Actions menu](./assets/action_menu.png)

Outputs list is dynamically build using [python-xlib](https://pypi.org/project/python-xlib/) api. Current primary output is marked with a "`*`".   
> Note : only connected outputs are displayed.

After output is selected, a new menu ask for action. 

Actions are : 
- `Disable` : Turn off selected output
- `Alone` : Keep only selected output on and turn off all others
- `Primary` : Set this output as primary output
- `Right of xxx` : Setup selected output to the **right** of current primary output
- `Left of xxx` : Setup selected output to the **left** of current primary output
- `Above of xxx` : Setup selected output to the **above** of current primary output
- `Below of xxx` : Setup selected output to the **below** of current primary output