<!-- give your annotation a title -->
# Paste Annotation

<!-- specify the "type" for your annotation -->
> ### net.paste-app.clip

<!-- provide a description of what your annotation represents -->
A paste is a message in a paste channel (of type net.patter-app.clips) 
with an annotation of this type.

<!-- provide at least one example of what your annotation might look like in the wild -->
## Examples

~~~ js

"data":[
	{"annotations":[
		{
			"type":"net.paste-app.clip",
			"value":{
				"title":"Recent Paste Test",
				"content":"Testing insertion of new pastes into Recent Pastes, #5b.",
				"content_type":"text"
			}
		}
	],
	}
]
~~~

<!-- provide a complete description of the fields in the "value" object for your annotation -->
## Fields 

| Field | Required? | Type | Description |
| ----- | --------- | ---- | ----------- |
| `title` | Optional | string | Short user description of the clipping. |
| `content` | Optional | string | Main clipping text. |
| `content_type` | Optional | string | Programming language, including plain text, for help in formatting the clipping for display. |
| `tags` | Optional | list of strings | User-defined tag(s) for the clipping. |

## Notes

Pastes will display the remaining metadata if the content field is omitted, so no fields are required.  (Does ADN require a value?)

categories is a list of identifiers. The following identifiers are recognized by patter-app.net: 'fun', 'lifestyle', 'profession', 'language', 'community', 'tech', 'event'. If a channel does not have a recognized category, it should be listed as a 'general' room.

<!-- provide a way to contact you -->
## Maintainers
* [M. C. DeMarco](http://mcdemarco.net) ([@mcdemarco](https://alpha.app.net/mcdemarco))

<!-- provide references to compatible apps / service -->
## Used by
* [Paste](http://paste-app.net)

<!-- provide references to related annotations -->
## Related annotations

net.paste-app.settings
net.paste-app.clips
