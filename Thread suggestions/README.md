## Trigger
``` 
.*
```
## Command
```go
{{ if eq .Message.ID .Channel.ID}}
 	{{addReactions "❎" "✅"}}
	
 	{{ $embed := cembed "description" (print "Thank you, " .User.Username ". Suggestions help improve this Discord server.")}}
	{{ sendMessage nil $embed }}
{{ end }}
```

Make sure to make it only run in the thread channel needed.

## Resault
![Image shows discord, notably there's a thread post with x and check reactions, an embed by YAG saying "Thank you, paol. Suggestion help improve this Discord server.](../.imgs/Thread%20demo.webp)
