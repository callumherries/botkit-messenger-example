# Facebook Messenger Botkit Chatbot

An example [Facebook Messenger](https://messenger.com) node.js chatbot and integrated with [Dialog Analytics](https://dialoganalytics.com). Built with [howdyai/botkit](https://github.com/howdyai/botkit).

- [Dialog Documention](https://docs.dialoganalytics.com)
- [Dialog API reference](https://docs.dialoganalytics.com/reference)

## Getting started

Clone this repository and run `npm install`

Create an account on https://app.dialoganalytics.com, grab your Dialog API token and bot ID.

Follow [these instructions](https://github.com/howdyai/botkit/blob/master/readme-facebook.md#getting-started) to get started with a Messenger bot.

Set environment variables in `.env`:

```
FACEBOOK_PAGE_ACCESS_TOKEN=...
FACEBOOK_VERIFY_TOKEN=...
DIALOG_API_TOKEN=...
DIALOG_BOT_ID=...
```

__Local development:__ When developping locally, use a service like https://ngrok.com to expose a server running on your machine. You'll need to update your [Facebook app's webhook](https://developers.facebook.com/apps) and set it to something like `https://075301e2.ngrok.io/facebook/receive`.

```bash
$ ngrok http 3000
```

Start the bot:

```bash
$ node bot.js https://075301e2.ngrok.io
```

Open the Messenger application, find your bot and exchange a few messages. Messages will be sent to Dialog's API.

## Go further

Read more on how to make the most out of the possibilities offered by Dialog here: https://dialoganalytics.com
