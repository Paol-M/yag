Trigger
``` 
.*
```
Command
```go
{{ if eq .Message.ID .Channel.ID}}
 	{{addReactions "❎" "✅"}}
	
 	{{ $embed := cembed "description" (print "Thank you, " .User.Username ". Suggestions help improve this Discord server.")}}
	{{ sendMessage nil $embed }}
{{ end }}
```

Make sure to make it only run in the thread channel needed.