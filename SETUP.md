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

## Step 4 - Check If You Have Node.js

Node.js is a tool that lets you install Claude Code. You might already have it.

In your terminal, type this and press Enter:

```
node --version
```

- If you see something like `v20.0.0` — great, skip to Step 5
- If you see an error — go to **https://nodejs.org**, download the LTS version, install it, then come back here

---

## Step 5 - Install Claude Code

Claude Code is Claude inside your terminal. You type to it, it builds things for you.

In your terminal, type this exactly and press Enter:

```
npm install -g @anthropic-ai/claude-code
```

It will show a bunch of text scrolling — that's normal, just let it run. When it stops and you see a `$` or `>` symbol again, it's done.

---

## Step 6 - Get Your Pod API Key

An API key is like a password that lets Claude Code talk to Claude's brain. Your pod has one waiting for you.

1. Open Discord: **https://discord.gg/g2pJzjmV**
2. Find your Pod channel (Pod A, Pod B, Pod C, Pod D, or Pod E)
3. Your API key will be pinned there — it looks like this: `sk-ant-...`
4. Copy it (you'll need it in the next step)

---

## Step 7 - Start Claude Code for the First Time

In your terminal, type this and press Enter:

```
claude
```

The first time you run it, Claude Code will walk you through setup automatically. It will ask for your API key — paste the one you copied from Discord.

Follow the prompts on screen. It's straightforward.

When setup is done, you'll see a `>` prompt waiting for you. You're in.

---

## Step 8 - Load the Workshop Repo Into Claude Code

This is where the magic happens. When you open this repo inside Claude Code, it already knows everything about today's workshop — who you are, what you're building, how to help.

In your terminal, run these one at a time:

```
git clone https://github.com/arc-web/stellarph-claude-workshop.git
```

```
cd stellarph-claude-workshop
```

```
claude
```

Claude Code will start up and read the workshop context automatically. You're ready to build.

---

## You're All Set

Here's what you now have:

- Claude in your browser (claude.ai)
- Claude on your desktop (Claude Desktop app)
- Claude Code in your terminal (the most powerful one)
- Your pod's API key connected
- The workshop repo loaded and ready

**Your first prompt to get started:**

```
I'm at the StellarPH Claude AI Workshop. Help me figure out what to build today.
Ask me about my background, what problems I deal with at work, and what I'd love to automate or make easier.
```

---

## Useful Terminal Shortcuts

| What you want to do | How to do it |
|---------------------|-------------|
| Stop what's running | Press `Ctrl + C` |
| Clear the screen | Type `clear` and press Enter |
| Exit Claude Code | Press `Ctrl + C` or type `/exit` |
| Run Claude Code again | Type `claude` and press Enter |
| Go back a folder | Type `cd ..` and press Enter |

---

## Something Went Wrong?

**Claude Code says "command not found"**
Run `npm install -g @anthropic-ai/claude-code` again

**API key not working**
Make sure you copied the whole thing including the `sk-ant-` at the start. No spaces before or after.

**Node.js install didn't work**
Download it directly from https://nodejs.org (click the big LTS button)

**Anything else**
Post in your Pod channel on Discord. Someone's got you.

---

Back to [main README](README.md)
