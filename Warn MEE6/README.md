# MEE6 warn embed
Result
![Picture showing the result](https://i.ibb.co/0BH054d/yag-warn.png)

## You can follow this tutorial on YouTube

[How to embed a warn with YAGPDB](https://youtu.be/2LxMwg7fxl8)

## Step 1
Copy this code

    {{ $embed := cembed "description" (print "**Reason:** " .Reason) "author" (sdict "name" (print (toString .User.String) " has been warned") "icon_url" (.User.AvatarURL "256")) "color"  2960685}}
    
    {{ sendMessage nil $embed }}
    
    
    
    {{/* If you don't want the bot to DM the person getting warned delete this and everything under it */}}
    
      
    
    {{ sendDM $embed }}
## Step 2
Go to: **YAGPDB's control panel** > **moderation** *under “Tolls & Utilities”* > **Warnings** > **Warn DM**
![Image of the end result](https://i.ibb.co/bFwQkQ0/Screenshot.png)
You should end up here *code might look different*, **Make sure to save**
## Step 3
Paste the code you copied
## Step 4
Go to: **Command Settings** > **New command override** *at the bottom of the page* if you can't find it go to step **6** and check the image
## Step 5
Under *Apply to the following commands* select *Warn* 
## Step 6 
Set auto delete **response** to **0** and click the check icon
so it ends up looking like that
 - [x] 0
![End Result](https://i.ibb.co/8PXvfvr/Screenshot.png)
It should look like that, **make sure you save**

# You Should be done!
If it's not working you can check the YouTube video listed above and feel free to DM me on Discord [paol#7272](https://discordapp.com/users/573589702368821259).