# Create the voiceover

After you approve the storyboard, each cut needs a voice recording, called a *take*. ElevenLabs generates the takes. There are two ways to do it:

| Route | How it works | When it's available |
|---|---|---|
| [Through a connector](#generate-the-takes-through-a-connector) | Claude generates the takes for you, using an ElevenLabs tool connected to Claude. | Only when Claude has an ElevenLabs connector. To add one, see [Connect ElevenLabs to Claude](#connect-elevenlabs-to-claude-optional). |
| [By hand](#generate-the-takes-by-hand) | You paste the script into elevenlabs.io, generate the takes, and send Claude the files. | Always. |

Claude checks for a connector during the interview. If it finds one, it asks which route you want. If not, you use the by-hand route.

You never need to give Claude an ElevenLabs API key.

## Before you begin

Record the voice only when the script is final, because every change to the words needs a new recording. Make sure that:

- You've approved the storyboard. For details, see [Review and approve the storyboard](review-the-storyboard.md).
- You can sign in to [elevenlabs.io](https://elevenlabs.io).

## Choose a voice

Claude doesn't choose the voice for you. If you don't have a voice yet, choose one in the ElevenLabs voice library, or create one with Voice Design. Claude can write a Voice Design description for you, based on the tone you described. In ElevenLabs, a Professional Voice Clone performs best with the Eleven v4 model.

To give Claude a voice you already use, find its voice ID in ElevenLabs: go to **Voices**, select **⋯** next to the voice, and then select **Copy voice ID**. Paste the ID into your reply to Claude.

## Generate the takes by hand

You generate the takes at elevenlabs.io and send Claude the files.

### Set up the text-to-speech page

You do this once, before the first cut.

1. In elevenlabs.io, open the text-to-speech page.
2. Select the **Eleven v4** model. The script contains voice directions that only this model understands. Don't use a turbo model, because it ignores most of them.
3. Select the voice. If you haven't told Claude its name yet, tell Claude now, so Claude can record it for later takes.
4. Set **Stability** and **Similarity** to the values Claude gives you. If Claude gives you a seed number, enter it too.

### Generate a take for each cut

Repeat these steps for each cut that has its own recording. A vertical copy of a cut uses the same recording as the original, so it doesn't need its own take.

1. Copy the script that Claude gives you for the cut. It appears in a box, ready to paste.
2. Paste the whole script for the cut into the text box. Generate it in one piece, not paragraph by paragraph, so the voice stays consistent.
3. Generate three or four takes. Each take sounds a little different.
4. Listen to each take. Avoid any take that reads a direction aloud, such as saying "warm, assured," or that mispronounces your product name.
5. Download your favorite take as an MP3 file. If you can't choose, download several and let Claude pick the one that best matches the script.
6. Tell Claude which cut the file is for and where it is, for example:

   ```text
   The take for the 30-second cut is in ~/Downloads/cut30-take2.mp3
   ```

## Connect ElevenLabs to Claude (optional)

With a connector, Claude can generate the takes for you. You set it up once, and you don't need an API key.

1. In Claude, select your account icon in the lower-left corner, and then select **Settings**.
2. Select **Customize**, and then open the **Connectors** tab.
3. Find **ElevenLabs** in the list, or search for it.
4. Connect it.
5. Follow the instructions on the screen to sign in to ElevenLabs and allow access. In the Claude desktop app, you might be asked to continue in your browser.
6. Close Claude Code and open it again in your product's folder. Claude Code loads connectors only when it starts.
7. To check the connection, type `/mcp` in Claude Code. **ElevenLabs** should appear in the list.

   If **ElevenLabs** doesn't appear, check that you signed in to Claude Code with the same Claude account that you use in the Claude app.

The takes use the credits of your ElevenLabs account. On Team and Enterprise plans, only an admin can add connectors. For details, see [ElevenLabs MCP server](https://elevenlabs.io/docs/eleven-api/resources/mcp-server).

## Generate the takes through a connector

If your Claude session has an ElevenLabs connector, Claude can generate the takes for you. You choose the voice and listen to the result.

1. Tell Claude which voice to use, or ask Claude to find one that matches your description.
2. Claude generates three or four takes for each cut and picks the best match. Alternatively, Claude plays the takes for you, and you choose one.
3. Sometimes Claude can't save the audio as a file. In that case, Claude asks you to download the take you chose. Then tell Claude where the file is.

If the connector fails or can't use the Eleven v4 model, Claude tells you and switches to the by-hand route.

## What happens next

For each take, Claude:

1. Copies the file into the project and adjusts its volume to a standard level for web and social video. Your original file isn't changed.
2. Listens to the take and matches each word to the script, so the pictures move in time with the voice.
3. Reports how well the take matches the script. Above 90% is normal. Below 80% usually means the take doesn't match the current script.

   If a take doesn't match well, Claude tells you what to regenerate. For details, see [The voice take doesn't match the script](../troubleshooting.md#the-voice-take-doesnt-match-the-script).

## Next steps

- [Review and approve the final videos](review-the-final-videos.md)
- To record a new take later, see [Use a new voice take](change-a-video.md#use-a-new-voice-take).
