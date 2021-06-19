---
layout: single
title: Developer Sign-Up
permalink: /sign-up/
---

You're developing bots or userbots and want to be listed on this page! Sure thing. All you need to do is open a [pull request](https://github.com/TGBotDevList/tgbotdevlist.github.io/compare) on GitHub to add your information.

Obviously that information will then be public and I can't control who reads it. If you don't want that, don't open a pull request.

Let me walk you through the requirements for a sucessfull PR:

# Add yourself to [`_data/authors.yml`](https://github.com/TGBotDevList/tgbotdevlist.github.io/blob/main/_data/authors.yml)

You can copy the entry of `john_does_gh_username` and adjust it to your needs. Most fields can just be deleted if you don't need them.

```yml
# use your github username as slug
john_does_gh_username:
  name        : "John Doe" # Your real name or an alias
  bio         : "Short Bio."
  # To add a profile picture, add it as /assets/profile_pictures/your_gh_username.png or add a link
  avatar      : "/assets/profile_pictures/john_does_gh_username.png"
  links:
    # Any relevant social links. The only mandatory one is your GitHub profile.
    - label: "GitHub"
      # fontawesome icons are optional
      icon: "fab fa-fw fa-github"
      url: "https://github.com/tgdevbotlist/tgdevbotlist.github.io"
    - label: "Email"
      icon: "fas fa-fw fa-envelope-square"
      url: "mailto:john@doe.com"
    - label: "Website"
      icon: "fas fa-fw fa-link"
      url: "https://tgdevbotlist.github.io"
    - label: "Some Other Social Link"
      icon: "fas fa-comment"
      url: "https://github.com/tgdevbotlist/tgdevbotlist.github.io"
  # Which languages you code.
  languages:
    - name: "Python"
      # fontawesome icons are optional
      icon: "fab fa-python"
      # If you use specific packages for Telegram development in this language, list them here
      packages:
        - name: "python-telegram-bot"
          url: "https://python-telegram-bot.org"
    - name: "Rust"
  # Some references of yours. Must contain at least one item
  references:
    - name: "TwitterStatusBot"
      type: "bot"
      telegram: "TwitterStatusBot"
    - name: "SomeUserBot"
      type: "userbot"
      url: "https://core.telegram.org/"
    - name: "Reference without link"
      type: "bot"
```

## A note on authentication

In order for me to be able to verify that your information is legitimate, I make the following requirements:

1. The pull request must come from the same GitHub account that's used as author slug and linked in the social links
2. Any social link or references must be directly associated to your GitHub account. That means that e.g. the homepage you linked states that your GitHub account belongs to the owner of that homepage.
3. If you add a profile picture as file, it must be visible on one of your social accounts at the time of making the pull request. If you add a profile picture as link, the link must point to one of the social accounts linked by you.
4. The `name` you choose must also be clearly visible on one of your social accounts. Please tell me where I can find it.

# Add a post for yourself

Make a copy of [`_posts/2021-06-18-john_does_gh_username.md`](https://github.com/TGBotDevList/tgbotdevlist.github.io/blob/main/_posts/2021-06-18-john_does_gh_username.md) in the `_posts` directory and change the filename properly:

* The date should be (roughly) the date of your pull request (relevant in case you update your information)
* the rest of the filename must be your GitHub username

Then fill it with info:

```markdown
---
# use your github username as author
author: john_does_gh_username
# Your real name or an alias as title
title: John Doe
# Uncomment the ones that you can actually program
# For each of the two categories, you must include at least one reference
categories:
#    - userbot
#    - bot

# Use the tags for all languages that you code
tags:
#    - rust
#    - python
#    - some other language
---

# About Me

John Doe is just a placeholder and has no life. You instead may introduce yourself here in a short paragraph.

# Coding Interests

John Doe is mostly interested in bots that have a search functionality via the inline mode. He uses userbots only when strictly necessary. How about you?

# Conditions

If you have some conditions for commissions that apply generally, list them here. E.g.

* 25 Schmeckels/hours
* Fixed prices for bots with up to 5 commands without 3rd-party integrations
* Maybe you even have a contract template that you can link here?
```

And that's already it. I will review your information and get back to you as soon as I reasonably can.
