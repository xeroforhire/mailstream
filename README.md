# Mailstream

Your email as a scrollable feed instead of a list.

Each email shows up as a card, like a post: the sender where a profile picture would be, the subject, and a short preview. Tap a card to open the full email. Every card has four actions: **Reply**, **Forward**, **Not interested** and **Spam**.

What makes it different from a regular inbox is that it learns from what you tell it:

- **Spam blocks the whole company, not one address.** Mark one Northline email as spam and it also catches `news.northline.com`, `northline-mail.com`, `northlineoutfitters.com`, look-alike spellings and matching sender names. Personal addresses (Gmail, iCloud and so on) are only ever blocked one address at a time.
- **Not interested learns topics.** It picks up the key words and phrases from that email, like "flash sale" or "limited time." New mail that matches several of them goes to a **Filtered** tab instead of your feed. Nothing is deleted.
- **Anyone you reply to is trusted** and never filtered, so a real conversation can't get swept up by a promo rule.
- **What it learned** shows every blocked company, muted word and trusted sender, and lets you remove any of them. Every action can be undone.

## Status: prototype with sample mail

This version runs on **made-up sample emails**. It does not connect to a real inbox yet, and Reply and Forward don't send anything. It's for testing how the feed and the filters *feel*.

What it learns is saved in your own browser only. Nobody else sees it, and "Reset everything" on the **What it learned** tab starts over.

## Try it

Open `index.html` in any browser, or use the hosted link if one was shared with you. It works best on a phone.

A good first run:

1. Scroll the feed and open a few emails.
2. Tap **Not interested** on the Northline flash sale.
3. Tap **Spam** on the other Northline email.
4. Tap **Pull in new mail** and see what gets through and what gets caught.
5. Check the **Filtered**, **Spam** and **What it learned** tabs.

## Feedback we're looking for

- Does scrolling your mail like a feed feel better than a list, or just different?
- Is the preview the right length? Too short to tell what an email is about, or too long?
- Did the filter ever catch something you wanted, or miss something obvious?
- Did you reach for a swipe gesture? Which direction, and what did you expect it to do?
- Would you open this first thing in the morning instead of your email app? Why or why not?

## Roadmap

- Connect a real Gmail inbox
- Turn a Spam tap into a real Gmail filter
- Eddy, the in-app helper who explains what the filter learned and why
