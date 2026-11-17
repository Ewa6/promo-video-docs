# Set up the skill

This page takes you from nothing installed to a skill that's ready to make videos. You do this once per computer.

## Before you begin

Read [Before you begin](prerequisites.md) and make sure you have Claude Code, an ElevenLabs account, and the product's code on your computer.

## Step 1: Install the required tools

Claude Code runs the video tools on your computer, so they need to be installed first.

1. Open a terminal. On a Mac, open the **Terminal** app.
2. Check Node.js by running:

   ```bash
   node -v
   ```

   If the command isn't found, or the version is earlier than `v22.18.0`, install the current version from [nodejs.org](https://nodejs.org). npm is included.
3. Check git and make by running:

   ```bash
   git --version
   make --version
   ```

   On Windows, skip `make --version`: you don't need make.

   On a Mac, if either command isn't found, install the Xcode Command Line Tools:

   ```bash
   xcode-select --install
   ```

   Follow the window that opens, and then run the checks again.

You can also ask Claude to run these checks and tell you what's missing.

## Step 2: Choose where to install the skill

You can install the skill in one of two places:

| Option | Who gets the skill | Choose it when |
|---|---|---|
| For yourself | You, in every project on this computer | You make videos for more than one product. |
| For one product | Everyone who opens that product's folder in Claude Code | Your team shares the product folder and should all have the skill. |

If you're not sure, install it for yourself.

## Step 3: Get the skill

The skill isn't public. To use it, contact one of the authors on LinkedIn:

- [Ewa Jabłońska](https://www.linkedin.com/in/ejablonska/)
- [Krzysztof Jabłoński](https://www.linkedin.com/in/krzysztof-jab%C5%82o%C5%84ski/)

You get the skill files and the install command for the place you chose in Step 2.

## Step 4: Check that the skill is ready

1. If Claude Code is open, start a new session so it loads the skill.
2. Open Claude Code in your product's folder.
3. Type `/` and look for **promo-video** in the list.

If **promo-video** appears, the skill is installed and ready to use.

If it doesn't appear, see [The skill doesn't appear in Claude Code](troubleshooting.md#the-skill-doesnt-appear-in-claude-code).

## What happens the first time you make a video

You don't need to do anything else now. When you make your first video, Claude:

- creates the video project inside your product's folder;
- downloads the video tools, which needs an internet connection;
- builds the speech-timing tool (on Windows, downloads it ready-made). This takes about a minute and happens only once per computer.

## Update the skill

To get the latest version of the skill, contact the authors.

## Next steps

- [Quick start: make your first video](quick-start.md)
- To learn what happens at each stage, see [How a promo video gets made](how-it-works.md).
