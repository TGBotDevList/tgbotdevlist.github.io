---
layout: single
title: General Advice
permalink: /advice/
---

What follows it far from being legal advice. It's just some things that I personally consider common sense and that you should probably think of before wiring money to/starting to work for a stranger on the internet.

Are you missing something here? Please [tell me](https://github.com/TGBotDevList/tgbotdevlist.github.io/issues/new/choose).

# Bot functionality

* Both parties should be clear about what the bot is supposed to do. A short paragraph usually doesn't cut it. Consider setting up flow charts and writing the functionality down in detail.
* Communicate about the user experience design. E.g., should the bot use [ReplyKeyboardmarkups](https://core.telegram.org/bots/#keyboards) or rather [InlineKeyboardMarkups](https://core.telegram.org/bots/#inline-keyboards-and-on-the-fly-updating)?
* All bots should have proper exception handling. But who gets informed about exceptions at runtime? The client or the developer? Settle this.

# Payment

* You should settle on clear payment policies. This includes regulations for cases where the bot is done early or late or when client/developer decides on-the-fly that the bots needs additional functionality to be usable.
* The method of payment should be discussed beforehand, especially if client and developer don't use the same currency
* Time of payment is important, too. The developer may insist on getting a part of the payment upfront. The client may insist on testing the bot before paying the rest.

# Runtime

* It should be discussed if the developer is responsible for any bugfixes after the client has accepted the commission. If yes, you should consider to settle on terms for this event.
* Clients should be aware that writing the code for a bot and hosting that bot are two pairs of shoes. If you expect the developer to manage the hosting, you need to address this beforehand. In this case, settle on terms for how hosting is payed, how downtimes are handled etc.
