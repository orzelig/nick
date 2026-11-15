# Kid-Friendly Videos

A hand-picked video page for the kids: Scratch Garden songs, Nat Geo Kids, Mark Rober science, Nick DiGiovanni cooking and a few other learning channels.

Live: https://orzelig.github.io/nick/ · Part of the [Kids' Library](https://orzelig.github.io/kids-library/)

## Locked player

Videos play inside the page, not on YouTube:

- YouTube's own controls are hidden and a clear layer covers the video, so the title, logo, end cards and suggestions can't be tapped.
- Pausing shows the page's own cover, hiding YouTube's "More videos" strip.
- When a video ends, the page shows its own "That's the end!" screen with **Watch again** and picks from this list only.
- Videos load from `youtube-nocookie.com`.

## Adding a video

Add an entry to `videos.json`:

```json
{ "id": "dQw4w9WgXcQ", "title": "Video title", "channel": "Scratch Garden", "added": "2026-11-15" }
```

- `id` is the part after `v=` in the YouTube link.
- `channel` should be the real channel name. Scratch Garden, Nat Geo Kids, Mark Rober and Nick DiGiovanni get their own filter; any other channel goes under **More fun**.
- `added` (optional) shows a **NEW** badge for 30 days.

Check a video's real title and channel before adding it:

```bash
curl -s "https://www.youtube.com/oembed?format=json&url=https://www.youtube.com/watch?v=VIDEO_ID"
```

New uploads for a channel are in its feed, e.g. Scratch Garden: https://www.youtube.com/feeds/videos.xml?channel_id=UC8NFs-VWUsyuq4zaYVVMgCQ
