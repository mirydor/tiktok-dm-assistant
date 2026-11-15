# tiktok-dm-assistant

A Claude Code skill that watches your TikTok Business Suite inbox in Chrome:

- Replies `Няма проблем🙏` to thank-you messages automatically
- Drafts LitBuy answers to real questions and waits for your OK (with a phone notification)
- Flags collabs, unviewable media, customs and money problems
- Checks every minute while someone is chatting, every 10 minutes when it's quiet

## Install on your PC

1. Install the **Claude desktop app** and sign in.
2. Install **Chrome** + the **Claude in Chrome** extension, sign in to the same account, and log in to TikTok in that Chrome.
3. Copy this folder into your Claude skills folder:
   - Windows: `C:\Users\<you>\.claude\skills\tiktok-dm-assistant\`
   - (so that `SKILL.md` is at `...\.claude\skills\tiktok-dm-assistant\SKILL.md`)

   Easiest way from a terminal:
   ```
   git clone https://github.com/<your-user>/tiktok-dm-assistant.git "%USERPROFILE%\.claude\skills\tiktok-dm-assistant"
   ```
4. Open a Claude Code session in the desktop app and type `/tiktok-dm-assistant`.
5. Optional: turn on **Remote Control** for that session so approval alerts reach your phone.

## Keep it running 24/7

- Set Windows power settings so the PC never sleeps.
- Keep the Claude app and Chrome open.
- The loop lives in that session; if the app restarts, run `/tiktok-dm-assistant` again.

## Updating the bot answers

Edit `references/litbuy-bot-instructions.md` (the same file your other chatbot uses) and push. On the PC run `git pull` inside the skill folder.
