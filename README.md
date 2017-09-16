All webhooks come with the following structure:

```json
{
    "model": {
        "id": "597f3c854baa6e43db4f07d7",
        "name": "testing",
        "desc": "",
        "descData": null,
        "closed": false,
        "idOrganization": "597f2c1a80a903bf442c826e",
        "pinned": false,
        "url": "https://trello.com/b/CGKHU6vL/testing",
        "shortUrl": "https://trello.com/b/CGKHU6vL",
        "prefs": {
            "permissionLevel": "org",
            "voting": "disabled",
            "comments": "org",
            "invitations": "members",
            "selfJoin": true,
            "cardCovers": true,
            "cardAging": "regular",
            "calendarFeedEnabled": false,
            "background": "green",
            "backgroundImage": null,
            "backgroundImageScaled": null,
            "backgroundTile": false,
            "backgroundBrightness": "dark",
            "backgroundBottomColor": "#519839",
            "backgroundTopColor": "#519839",
            "backgroundColor": "#519839",
            "canBePublic": true,
            "canBeOrg": true,
            "canBePrivate": true,
            "canInvite": true
        },
        "labelNames": {
            "green": "",
            "yellow": "",
            "orange": "",
            "red": "",
            "purple": "",
            "blue": "",
            "sky": "",
            "lime": "",
            "pink": "",
            "black": ""
        }
    },
    "action": {
        "id": "59bc8e2ddbd7af0e1474fb0e",
        "idMemberCreator": "50e853a3a98492ed05002257",
        "data": {
            "checklistSource": {
                "name": "7777777777777",
                "id": "59bc8e1b5135cbe9718deb2d"
            },
            "board": {
                "shortLink": "CGKHU6vL",
                "name": "testing",
                "id": "597f3c854baa6e43db4f07d7"
            },
            "checklist": {
                "name": "7777777777777",
                "id": "59bc8e2ddbd7af0e1474fb08"
            }
        },
        "type": "copyChecklist",
        "date": "2017-09-16T02:36:29.244Z",
        "memberCreator": {
            "id": "50e853a3a98492ed05002257",
            "avatarHash": "d2f9f8c8995019e2d3fda00f45d939b8",
            "fullName": "Giovanni P",
            "initials": "FJ",
            "username": "fiatjaf"
        },
        "display": {
            "translationKey": "unknown",
            "entities": {
                "memberCreator": {
                    "type": "member",
                    "id": "50e853a3a98492ed05002257",
                    "username": "fiatjaf",
                    "text": "Giovanni P"
                }
            }
        }
    }
}
```

`model` is the model being observed. `action` is different depending on the event type. Each type of event has its structure in one file in this repository.
