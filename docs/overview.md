# What the promo video skill does

The promo video skill lets Claude make narrated marketing videos for a software product. It works from the product's own code, website, and brand, so the videos show your real product, your real colors, and the words your customers already know.

You don't need video-editing skills. Claude does the research, writing, animation, and checking. You make the decisions: what the video says, how it sounds, and whether it's ready.

## What you get

By default, Claude makes four versions of the video. Each version is called a *cut*.

| Cut | Length | Shape | Captions | Typical use |
|---|---|---|---|---|
| Main video (hero) | About 60–90 seconds | Landscape | Off | Website, LinkedIn, trade-show screens |
| 30-second cut | About 30 seconds | Landscape | On | Paid social posts, video ads |
| 15-second cut | About 15 seconds | Landscape | On | Stories, event loops |
| 15-second vertical cut | About 15 seconds | Vertical (phone) | On | Phone-first feeds |

You can ask for different lengths, shapes, or a different set of cuts during the interview. For details, see [Change a finished video](how-to/change-a-video.md).

Each cut is an MP4 video file with:

- A voiceover that you generate with ElevenLabs, an AI voice service
- Animated scenes that move in time with the voice
- Recreated screens of your product, filled with realistic but invented data
- Your logo, colors, and call to action at the end
- Word-by-word captions on the shorter cuts, for people who watch with the sound off

Claude also gives you a storyboard image for each cut, so you can check the whole video at a glance.

## Who it's for

The skill is for people who need a product video and have access to the product's code. For example:

- Founders and product managers who want a launch or explainer video
- Marketing teams who want consistent videos in several lengths
- Anyone who needs to update an existing promo video, for example with a new voice or shorter cut

You don't need to write code. Claude runs every technical step. You might need someone to help you install a few free tools the first time. For details, see [Before you begin](prerequisites.md).

## What it doesn't do

- **It doesn't record the voice for you without ElevenLabs.** You need an ElevenLabs account. Claude writes the script and the voice settings, and you (or a connected ElevenLabs tool) generate the recording.
- **It doesn't invent claims.** Every line in the script comes from your product, your website, or your answers. Numbers appear only when you can name their source.
- **It doesn't use real customer data.** Product screens are recreated with invented data. Screenshots are taken only from a demo version of your app.
- **It isn't a general video editor.** It makes motion-graphics promo videos for software products. It doesn't edit live-action footage, although you can add your own clips. For details, see [Add screenshots, footage, or music](how-to/add-screenshots-footage-music.md).

> [!IMPORTANT]
> The videos are built with Remotion. Remotion is free only for individuals, companies with up to three people, and non-profit organizations. Other companies need a [Remotion Company License](https://www.remotion.dev/license). For a promo video, you also need a paid ElevenLabs plan, because the Free plan allows only non-commercial use.

## Next steps

- To learn the stages Claude follows and where you take part, see [How a promo video gets made](how-it-works.md).
- To check whether you're ready to start, see [Before you begin](prerequisites.md).
