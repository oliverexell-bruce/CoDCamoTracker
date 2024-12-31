# Call of Duty Camo Tracker
Use this HTML file to help track which camos you're up to.

![image](https://github.com/user-attachments/assets/c8867377-3a7c-48ad-aad6-0abc0a3199c1)

It automatically saves when you change a colour or click a checkbox, so you can close and reopen it whenever.

<br />

## Tabs
There's 3 tabs up the top, zombies is the default.\
To change the default tab, find the folling line at the bottom of the file. 

```document.getElementsByClassName('tablinks')[1].click();```

Simply change the '1' to change the default tab. 

0 - Multiplayer\
1 - Zombies\
2 - Warzone

## Colours
You can change the colour of a gun by right clicking on its name.\
Each colour corresponds to a different amount of progress towards the camos

Black - No Progess\
Green - Military Camos\
Blue - Special 1\
Red - Special 2\
Purple - Both Specials\
Gold - Gold\
Silver - Diamond

For Dark Spine I use the checkbox + purple and for Dark Matter I use Checkbox + Black

Feel free to change the colours (the gold is fine on my second monitor but it's hard to read on the main one)

Just change the RGB values (in both places) near the bottom of the file here\
![image](https://github.com/user-attachments/assets/a1af7601-1f86-46b7-b5cc-2422b8f4be86)


## Adding More Weapons
Adding weapons is pretty straight forward\
Simply copy a line from an existing weapon\
```<label><input type="checkbox" id="mp-asval"> AS VAL</label><br><br>```
<br />

Give it a new ID and name (make sure it has the correct game mode)\
```<label><input type="checkbox" id="mp-krig"> KRIG C</label><br><br>```
<br />

Remove the second line break from the previous weapon\
```<label><input type="checkbox" id="mp-asval"> AS VAL</label><br>```

Finally, copy it into the other 2 game modes.

The counter's the total is automatically increased when a new weapon is added (it just counts the number of checkboxes on the page).

The reason this is required instead of just 1 list of all the weapons you need to edit is mostly because I'm lazy.\
I hard coded every weapon in for my first version (while I was trying to learn everything still) and now I can't be bothered fixing it.

## Unimportant Stuff
Originally it was to check off which weapons were gold/diamond since multiplayer queues allow for checking special camos, hence the checkboxes.\
However, after my friends and I started the zombies camos there was now a need to know progress without leaving the game, so I added the colours.

I figured I would use the checkbox and colours for Dark Spine and Dark Matter rather than adding colours for them (I am lazy).
