# Mailstream

Your email as a scrollable feed instead of a list.

Each email shows up as a card, like a post: the sender where a profile picture would be, the subject, and a short preview. Tap a card to open the full email. Every card has six actions: **OK**, **Save**, **Reply**, **Delete**, **Not interested** and **Spam**. **Forward** is at the top of the full email.

- **OK** means you've seen it. It archives the email, the same as archiving in Gmail.
- **Delete** throws it away (to Gmail's Trash) without teaching Mailstream anything.
- **Save** keeps it for later in the **Saved** tab. In Gmail it's starred, so it also shows up in Gmail's Starred folder.

What makes it different from a regular inbox is that it learns from what you tell it:

- **Spam blocks the whole company, not one address.** Mark one Northline email as spam and it also catches `news.northline.com`, `northline-mail.com`, `northlineoutfitters.com`, look-alike spellings and matching sender names. Personal addresses (Gmail, iCloud and so on) are only ever blocked one address at a time.
- **Not interested learns topics, not senders.** It picks up the key words and phrases from the subject and opening, like "flash sale" or "limited time." It ignores the sender's name and platform words like "Substack" or "subscribe," so muting one newsletter's topic doesn't mute every newsletter. New mail that matches several of them goes to a **Filtered** tab instead of your feed. Nothing is deleted.
- **Anyone you reply to or save from is trusted** and never filtered, so a real conversation can't get swept up by a promo rule.
- **What it learned** shows every blocked company, muted word and trusted sender, and lets you remove any of them. Every action can be undone.

## Status: private testing

Mailstream can sign in to a real Gmail account, or run on **made-up sample mail** if you just want to look around.

With Gmail connected:
- The feed shows your latest 40 inbox emails. Opening one marks it read in Gmail.
- **OK** archives the email in Gmail. **Save** stars it and archives it, and the **Saved** tab shows your starred emails.
- **Reply** and **Forward** really send. Forward sends the text of the email; attachments aren't included yet.
- **Spam** moves that email to Gmail's Spam folder. Other emails from the same company are held in Mailstream's Spam tab and left alone in Gmail.
- **Not interested** only changes Mailstream. Nothing moves in Gmail.

**Privacy:** there is no Mailstream server. Your mail goes straight from Google to your browser, and what Mailstream learns is saved in that browser only. Nobody else, including the person who shared the link, can see your email. You can remove Mailstream's access at [myaccount.google.com/permissions](https://myaccount.google.com/permissions).

Because Mailstream is in private testing, only people added as testers can sign in, and Google will warn that the app "hasn't verified" it. Tap **Advanced**, then **Go to Mailstream**. Sign-in lasts about an hour, then Mailstream asks you to sign in again.

## Try it

Open **https://xeroforhire.github.io/mailstream/** on your phone. Sign in with Google, or tap **Try it with sample mail**.

A good first run with sample mail:

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

- Load more than the latest 40 emails as you scroll
- Forward attachments
- Turn a Spam tap into a real Gmail filter
- Eddy, the in-app helper who explains what the filter learned and why
