# Custom-bossbar-addon ![download](https://img.shields.io/github/downloads/Gotemba912/Custom-bossbar-addon/total?style=plastic)  
This addon allows you to create your own bossbar !!!  

> ⚠Caution.  
> Using this addon, you will not be able to use vanilla bossbar or scoreboard sidebar.

★日本語版のREADMEを見る場合はここからどうぞ: [README.md](https://github.com/Gotemba912/Custom-bossbar-addon/README.md)

# How to use
After applying the resource pack to your world, run the following command to create an objective.  
★`<ID>` must be an arbitrary ID.
```
/scoreboard objectives add <ID> dummy
```
Next, display the objective in the sidebar.
```
/scoreboard objectives setdisplay sidebar <ID>
```

Now you are ready!  
Try to put any value in the objective.  
The boss bar will appear at the top of the screen!

# Set the maximum value
By default, the range is set to 0-100.

If you want to change the maximum value, you  
you will need to edit the pack file.  
First, change the UUID in `manifest.json`.  
*This is because it will be duplicated if this pack is applied on other servers.  

Once changed, open `hud_screen.json` in the `ui` folder with a text editor.

Line 34.
```
"$bossbar_max_value": 100.0,
```
This is where you set the maximum value.  
Set this to any value you wish.

> ⚠When setting the maximum value, be sure to add .0.

Example of setting:
```
"$bossbar_max_value": 32767.0,
```
Don't forget to save your changes!

You must exit and re-enter the world to apply the settings.

# Use the pack
You are free to incorporate this pack into your own packs.  
However, you must indicate that it was copied from this pack!

# License
[Licence.txt](https://github.com/Gotemba912/Custom-bossbar-addon/Licence.txt)

# Creator
@Gotemba912 (YukaYama0311)