# Set up the skill

This page takes you from nothing installed to a skill that's ready to make videos. You do this once per computer.

## Before you begin

Read [Before you begin](prerequisites.md) and make sure you have Claude Code, an ElevenLabs account, and the product's code on your computer.

## Step 1: Get the skill

The skill isn't public. To use it, contact one of the authors on LinkedIn:

- [Ewa Jabłońska](https://www.linkedin.com/in/ejablonska/)
- [Krzysztof Jabłoński](https://www.linkedin.com/in/krzysztof-jab%C5%82o%C5%84ski/)

## Step 2: Install the required tools

Claude runs the video tools on your computer, so a few programs must be installed first. Claude can check and install them for you.

1. Open Claude Code.
2. Type a request, for example:

   ```text
   Check that this computer has the tools for the promo video skill: Node.js 22.18 or later, Git, and Make. Install anything that's missing.
   ```

3. Read what Claude plans to install, and approve it.

On a Mac, an installer window for the Xcode Command Line Tools might open. Follow the steps in the window, and then tell Claude when it's done.

## Step 3: Choose where to install the skill

You can install the skill in one of two places:

| Option | Who gets the skill | Choose it when |
|---|---|---|
| For yourself | You, in every project on this computer | You make videos for more than one product. |
| For one product | Everyone who opens that product's folder in Claude Code | Your team shares the product folder and should all have the skill. |

If you're not sure, install it for yourself.

Ask Claude Code to install the skill files in the place you chose.

## Step 4: Check that the skill is ready

1. If Claude Code is open, start a new session so it loads the skill.
2. Open Claude Code in your product's folder.
3. Type `/` and look for **promo-video** in the list.

If **promo-video** appears, the skill is installed and ready to use.

If it doesn't appear, see [The skill doesn't appear in Claude Code](troubleshooting.md#the-skill-doesnt-appear-in-claude-code).

## What happens the first time you make a video

You don't need to do anything else now. When you make your first video, Claude:

- Creates the video project inside your product's folder.
- Downloads the video tools, which needs an internet connection.
- Builds the speech-timing tool (on Windows, downloads it ready-made). This takes about a minute and happens only once per computer.

## Update the skill

To get the latest version of the skill, contact the authors.

## Next steps

- [Quick start: make your first video](quick-start.md)
- To learn what happens at each stage, see [How a promo video gets made](how-it-works.md).
