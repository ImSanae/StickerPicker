# Sanae's collection of Matrix sticker packs

> [Preview address](https://matrix-stickers.pages.dev/)

## How to use this?

This picker only supports Element (Web, Electron, Android, iOS) clients as well as clients based on it.

Type `/devtools` in any chat window of your Element (web or desktop) and send it, a Developer Tools window will open, select `Explore account data`, find `m.widgets` in it and add the following to the "content":

```
{
    "stickerpicker": {
        "content": {
            "type": "m.stickerpicker",
            "url": "https://matrix-stickers.pages.dev/?theme=$theme",
            "name": "Stickerpicker",
            "creatorUserId": "@you:matrix.server.name",
            "data": {}
        },
        "sender": "@you:matrix.server.name",
        "state_key": "stickerpicker",
        "type": "m.widget",
        "id": "StickerPicker"
    }
}
```

If m.widgets is not found, select `Explore account data` event directly in the bottom right corner, select `Send custom account data event` for the event type and fill in:


```
{
  "type": "m.widgets",
  "content": {
    "stickerpicker": {
      "content": {
        "type": "m.stickerpicker",
        "url": "https://matrix-stickers.pages.dev/?theme=$theme",
        "name": "Stickerpicker",
        "creatorUserId": "@you:matrix.server.name",
        "data": {}
      },
      "sender": "@you:matrix.server.name",
      "state_key": "stickerpicker",
      "type": "m.widget",
      "id": "StickerPicker"
    }
  }
}
```
The same account should only need to be set up once.

## I'd like to add other stickers!

You can fork this repository and follow the [Wiki](https://github.com/maunium/stickerpicker/wiki/Creating-packs) prompts to import new stickers.The repository welcomes new sticker requests, so please initiate Pull Requests (from A to Z) by sorting the links to the original sticker pack.

Note: The repository does not accept stickers that contain explicit pornographic content.