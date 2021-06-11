# MEE6 warn embed
Result
![Picture of the result](https://i.ibb.co/0BH054d/yag-warn.png)

## You can follow this tutorial on YouTube

*coming soon*

## Step 1
Copy this code

    {{ $embed := cembed "description" (print "**Reason:** " .Reason) "author" (sdict "name" (print (toString .User.String) " has been warned") "icon_url" (.User.AvatarURL "256")) "color"  2960685}}
    
    {{ sendMessage nil $embed }}
    
      
    
    {{/* If you don't want the bot to DM the person getting warned delete this and everything under it */}}
    
      
    
    {{ sendDM $embed }}
## Step 2
Go to: **YAGPDB's control panel** > **moderation** *under “Tolls & Utilities”* > **Warnings** > **Warn DM**
![Image of the end resault](https://i.ibb.co/bFwQkQ0/Screenshot.png)
You should end up here, **Make sure to save**
## Step 3
Paste the code you copied
## Step 4
Go to: **Command Settings** > **New command override** *at the bottom of the page* if you can't find it go to step **6** and check the image
## Step 5
Under *Apply to the following commands* select *Warn* 
## Step 6 
Set auto delete **response** to **0** and click the check icon
 - [x] so it ends up looking like that
 ![End Resault](https://i.ibb.co/8PXvfvr/Screenshot.png)
It should look like that, **Make sure to save**