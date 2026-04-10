# Setup Guide

Follow these steps in order. Takes about 10 minutes. You only need to do this once.

If you get stuck at any point, drop a message in your Pod channel on Discord and someone will help.

---

## Step 1 - Get Claude in Your Browser

This is the easiest one. Just open a tab.

Go to **https://claude.ai** and create a free account if you don't have one yet.

That's it. Keep that tab open — you'll use it throughout the day.

---

## Step 2 - Download Claude Desktop

Claude Desktop is the same as the browser version, but it lives on your computer so it's always one click away.

1. Go to **https://claude.ai/download**
2. Download the version for your computer (Mac or Windows)
3. Open the downloaded file and install it like any normal app
4. Sign in with the same account you just made

You now have Claude on your computer. Nice.

---

## Step 3 - Open Your Terminal

The terminal is just a text window where you type commands to your computer. It sounds scary, it isn't.

**On Mac:**
- Press `Command + Space` to open Spotlight
- Type `Terminal` and press Enter
- A black or white window opens — that's it, you're in

**On Windows:**
- Press `Windows key + R`
- Type `cmd` and press Enter
- Or search for `Windows Terminal` in the Start menu

Keep this window open. You'll use it in the next steps.

---

## Step 4 - Get Your Pod API Key

Before you install anything, grab your API key. Think of it like a key that unlocks Claude Code for your pod today.

1. Open Discord: **https://discord.gg/g2pJzjmV**
2. Find your Pod channel (Pod A, Pod B, Pod C, Pod D, or Pod E)
3. Your API key will be pinned there — it starts with `sk-ant-`
4. Copy it and keep it handy

---

## Step 5 - Install Claude Code

Claude Code is Claude inside your terminal. You type to it in plain English and it helps you build things.

In your terminal, paste this and press Enter:

**Mac / Linux:**
```
curl -fsSL https://claude.ai/install.sh | bash
```

**Windows** (in Windows Terminal or PowerShell):
```
winget install Anthropic.ClaudeCode
```

You'll see some text scroll by — that's normal. Wait for it to finish.

---

## Step 6 - Add Your API Key

Before you start Claude Code, tell your terminal about your pod's API key. This is a one-time step.

**Mac / Linux** — paste this into your terminal, replacing `YOUR-KEY-HERE` with the key you copied from Discord:
```
export ANTHROPIC_API_KEY=YOUR-KEY-HERE
```

**Windows** — paste this, replacing `YOUR-KEY-HERE`:
```
set ANTHROPIC_API_KEY=YOUR-KEY-HERE
```

Press Enter. Nothing dramatic happens — that's fine, it worked.

---

## Step 7 - Load the Workshop Repo

This repo has workshop context built in. When Claude Code opens inside it, it already knows what today is about and how to help you.

Run these one at a time:

```
git clone https://github.com/arc-web/stellarph-claude-workshop.git
```

```
cd stellarph-claude-workshop
```

---

## Step 8 - Start Claude Code

Now just type:

```
claude
```

Claude Code will start up. It will show you a welcome screen and walk you through anything it needs from there — just follow what it shows you on screen. It's designed to guide you through itself.

When you see a `>` prompt, you're in and ready to go.

---

## You're All Set

Here's what you now have:

- Claude in your browser (claude.ai)
- Claude on your desktop (Claude Desktop app)
- Claude Code in your terminal — the most powerful one, loaded with workshop context
- Your pod's API key connected

**Your first prompt to get started:**

```
I'm at the StellarPH Claude AI Workshop. Help me figure out what to build today.
Ask me about my background, what problems I deal with at work, and what I'd love to automate or make easier.
```

---

## Useful Terminal Shortcuts

| What you want to do | How to do it |
|---------------------|-------------|
| Stop what's running | `Ctrl + C` |
| Clear the screen | Type `clear` then Enter |
| Exit Claude Code | Type `/exit` then Enter |
| Start Claude Code again | Type `claude` then Enter |
| Go back a folder | Type `cd ..` then Enter |

---

## Something Went Wrong?

**"command not found: claude" after installing**
Close your terminal, open a new one, and try `claude` again. If still broken, post in your Pod channel.

**API key not working**
Make sure you copied the whole key including `sk-ant-` at the start, with no spaces before or after.

**Git not installed (clone step failed)**
Download it from **https://git-scm.com/downloads** and run the setup again from Step 7.

**Anything else**
Post in your Pod channel on Discord. Someone's got you.

---

Back to [main README](README.md)
