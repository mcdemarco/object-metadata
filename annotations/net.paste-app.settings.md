<!-- give your annotation a title -->
# Paste Channel Settings

<!-- specify the "type" for your annotation -->
> ### net.paste-app.settings

<!-- provide a description of what your annotation represents -->
Paste channels may have an optional settings annotation to track
the user's paste tags and sections.

<!-- provide at least one example of what your annotation might look like in the wild -->
## Examples

~~~ js
{
    "type":"net.paste-app.clips",
    "annotations":[
      {
        "type":"net.paste-app.settings",
        "value":{
          "tags":[
            "tech","ponies"
          ],
          "sections":[
            "tech"
          ]
        }
      }
    ]
  }
}
~~~

<!-- provide a complete description of the fields in the "value" object for your annotation -->
## Fields 

| Field | Required? | Type | Description |
| ----- | --------- | ---- | ----------- |
| `tags` | Optional | list of strings | Zero or more identifiers the user has used to categorize their pastes. |
| `sections` | Optional | list of strings | Zero or more of the user's tags intended for grouping of pastes in the UI. |

## Notes

Tags are free-form and user-determined; sections are used by the app to aid in the display of pastes.
Applications should keep the sections list up-to-date and may update the tags list for tag auto-completion or other purposes. 

<!-- provide a way to contact you -->
## Maintainers
* [M. C. DeMarco](http://mcdemarco.net) ([@mcdemarco](https://alpha.app.net/mcdemarco))

<!-- provide references to compatible apps / service -->
## Used by
* [Paste](http://paste-app.net)

<!-- provide references to related annotations -->
## Related annotations

net.paste-app.clip
net.paste-app.clips
