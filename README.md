# Social media specs

Character limits, image sizes and 9:16 safe zones for every major social network, in one place and in JSON.

Last updated: 2026-10-29. Maintained by [Mydrop](https://mydropai.com/), the social media OS for agencies and multi-brand teams.

- [Caption character limits](#caption-character-limits): 10 networks
- [Image sizes](#image-sizes): 37 formats on 10 networks
- [Safe zones for Reels, Stories, TikTok and Shorts](#safe-zones-for-vertical-video)
- [Use the data](#use-the-data): `data/*.json`, free to reuse (MIT)

## Caption character limits

| Network | Max characters | Shown before "more" | Max hashtags | How it counts | Free counter |
|---|---:|---:|---:|---|---|
| Instagram | 2,200 | 125 | 5 | Unicode code points (an emoji counts as 1) | [Count](https://mydropai.com/tools/instagram-character-counter/) |
| TikTok | 2,200 |  |  | UTF-16 code units (an emoji or a CJK character counts as 2) | [Count](https://mydropai.com/tools/tiktok-character-counter/) |
| LinkedIn | 3,000 | 210 |  | Unicode code points (an emoji counts as 1) | [Count](https://mydropai.com/tools/linkedin-character-counter/) |
| X | 280 |  |  | Weighted: CJK and most emoji count as 2, any link counts as 23 | [Count](https://mydropai.com/tools/twitter-character-counter/) |
| Facebook | 63,206 |  |  | Unicode code points (an emoji counts as 1) | [Count](https://mydropai.com/tools/facebook-character-counter/) |
| Threads | 500 |  | 1 | Unicode code points (an emoji counts as 1) | [Count](https://mydropai.com/tools/threads-character-counter/) |
| Bluesky | 300 |  |  | Unicode code points (an emoji counts as 1) | [Count](https://mydropai.com/tools/bluesky-character-counter/) |
| YouTube | 5,000 |  |  | Unicode code points (an emoji counts as 1) | [Count](https://mydropai.com/tools/youtube-description-character-counter/) |
| Pinterest | 800 |  |  | Unicode code points (an emoji counts as 1) | [Count](https://mydropai.com/tools/pinterest-character-counter/) |
| Google Business Profile | 1,500 |  |  | Unicode code points (an emoji counts as 1) | [Count](https://mydropai.com/tools/google-business-profile-character-counter/) |

"Shown before more" is roughly where the feed cuts a caption on desktop. Check every network at once with the [free social media character counter](https://mydropai.com/tools/social-media-character-counter/).

## Image sizes

Recommended upload sizes, checked against each network's own help centre and developer docs. Networks rescale anything larger and soften anything smaller. When a network names only a range, the size here is the common choice inside it.

### Instagram

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Portrait post | 1080 x 1350 | 4:5 | Best feed size. Instagram's publishing API takes 4:5 to 1.91:1. |
| Tall portrait | 1080 x 1440 | 3:4 | Fills the profile grid since 2025. Tools that post through the API may crop it to 4:5. |
| Square post | 1080 x 1080 | 1:1 | Shows whole in the feed; the 3:4 grid trims its sides. |
| Landscape post | 1080 x 566 | 1.91:1 | The smallest image in the feed. |
| Story or Reel | 1080 x 1920 | 9:16 | Stories and Reels. Keep text out of the top 14%, the bottom 35% and 6% on each side. |
| Profile picture | 320 x 320 | 1:1 | Shown as a circle. |

Resize a photo to these sizes: [free Instagram image resizer](https://mydropai.com/tools/instagram-image-resizer/)

### Facebook

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Portrait post | 1080 x 1350 | 4:5 | Recommended for the feed; 1.91:1 to 4:5 is supported. |
| Square post | 1080 x 1080 | 1:1 | Shows whole in the feed. |
| Link preview | 1200 x 630 | 1.91:1 | Link previews. 600 × 315 is the minimum for the large card. |
| Story or Reel | 1080 x 1920 | 9:16 | Stories and Reels, with the same safe zone as Instagram. |
| Page cover | 851 x 315 | 2.7:1 | The size Facebook's help gives. The cover shows wider on desktop and shorter on phones: keep text in the middle. |
| Profile picture | 320 x 320 | 1:1 | Shown as a circle. |

Resize a photo to these sizes: [free Facebook image resizer](https://mydropai.com/tools/facebook-image-resizer/)

### LinkedIn

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Square post | 1080 x 1080 | 1:1 | Posts take 3:1 to 4:5, up to 20 photos, 5 MB each. |
| Portrait post | 1080 x 1350 | 4:5 | The tallest post image LinkedIn shows uncropped. |
| Landscape or link | 1200 x 627 | 1.91:1 | Link previews and landscape posts. |
| Profile banner | 1584 x 396 | 4:1 | Personal profile background, up to 8 MB. |
| Company Page cover | 1512 x 256 | 5.9:1 | Company Page cover, up to 3 MB. |
| Article cover | 1920 x 1080 | 16:9 | Article and newsletter cover. |
| Profile photo or logo | 400 x 400 | 1:1 | Profile photo or Company Page logo. |

Resize a photo to these sizes: [free LinkedIn image resizer](https://mydropai.com/tools/linkedin-image-resizer/)

### X

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Landscape post | 1600 x 900 | 16:9 | Standard ratios show uncropped on phones; very tall or wide images are centre-cropped. |
| Square post | 1080 x 1080 | 1:1 | Shows whole in the feed. |
| Portrait post | 1080 x 1350 | 4:5 | Shows whole in the feed on phones. |
| Header | 1500 x 500 | 3:1 | About 60 px at the top and bottom may be cut. |
| Profile picture | 400 x 400 | 1:1 | Shown as a circle, up to 2 MB. |

Resize a photo to these sizes: [free X image resizer](https://mydropai.com/tools/twitter-image-resizer/)

### TikTok

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Video or photo | 1080 x 1920 | 9:16 | Videos and photo mode, up to 35 photos. |

Resize a photo to these sizes: [free TikTok image resizer](https://mydropai.com/tools/tiktok-image-resizer/)

### YouTube

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Thumbnail | 1280 x 720 | 16:9 | Works everywhere under 2 MB. YouTube now takes up to 3840 × 2160 and 50 MB on desktop. |
| Channel banner | 2560 x 1440 | 16:9 | Keep text and logos inside the central 1546 × 423, the part every screen shows. |
| Shorts | 1080 x 1920 | 9:16 | Vertical video, up to 3 minutes. |

Resize a photo to these sizes: [free YouTube image resizer](https://mydropai.com/tools/youtube-image-resizer/)

### Pinterest

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Standard pin | 1000 x 1500 | 2:3 | Anything taller than 2:3 may be cut off in the feed. |
| Square pin | 1000 x 1000 | 1:1 | Supported, but takes less room than 2:3. |

Resize a photo to these sizes: [free Pinterest image resizer](https://mydropai.com/tools/pinterest-image-resizer/)

### Threads

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Portrait post | 1440 x 1920 | 3:4 | Threads shows 3:4 in the feed. |
| Square post | 1080 x 1080 | 1:1 | Shows whole in the feed. |

Resize a photo to these sizes: [free Threads image resizer](https://mydropai.com/tools/threads-image-resizer/)

### Bluesky

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Post image | 1600 x 900 | 16:9 | Any ratio works. Up to 4 images per post, under 2 MB each. |
| Profile banner | 1500 x 500 | 3:1 | Profile banner, under 1 MB. |
| Profile picture | 1000 x 1000 | 1:1 | Profile picture, under 1 MB. |

Resize a photo to these sizes: [free Bluesky image resizer](https://mydropai.com/tools/bluesky-image-resizer/)

### Google Business Profile

| Format | Size (px) | Ratio | Good to know |
|---|---|---|---|
| Photo or logo | 720 x 720 | 1:1 | Photos, cover and logo: 250 × 250 minimum, 10 KB to 5 MB. |
| Post image | 1200 x 900 | 4:3 | Google publishes no post size; 4:3 is the common choice. |

Resize a photo to these sizes: [free Google Business Profile image resizer](https://mydropai.com/tools/google-business-profile-image-resizer/)

All networks in one tool: [free social media image resizer](https://mydropai.com/tools/social-media-image-resizer/).

## Safe zones for vertical video

Pixels to keep free of text, logos and faces on a 1080 x 1920 frame, so the app's buttons and captions never cover them. The right edge clears each app's like, comment and share buttons.

| Format | Top | Bottom | Left | Right | Safe area | Source |
|---|---:|---:|---:|---:|---|---|
| Instagram Reels | 250 | 420 | 65 | 140 | 875 x 1250 | [Mydrop size guide](https://mydropai.com/post/social-media-image-and-video-sizes-2026/) |
| Instagram Reels (ad) | 269 | 672 | 65 | 140 | 875 x 979 | [Meta Ads Guide](https://www.facebook.com/business/ads-guide/update/video/instagram-reels) |
| Instagram Stories | 269 | 672 | 65 | 65 | 950 x 979 | [Meta Ads Guide](https://www.facebook.com/business/ads-guide/update/video/instagram-reels) |
| TikTok | 130 | 350 | 40 | 180 | 860 x 1440 | [Mydrop size guide](https://mydropai.com/post/social-media-image-and-video-sizes-2026/) |
| YouTube Shorts | 288 | 672 | 48 | 192 | 840 x 960 | [Google Ads Help](https://support.google.com/google-ads/answer/9128498) |
| Facebook Reels & Stories | 269 | 672 | 65 | 140 | 875 x 979 | [Meta Ads Guide](https://www.facebook.com/business/ads-guide/update/video/instagram-reels) |

Check your own frame: [free safe zone checker](https://mydropai.com/tools/social-media-safe-zone-checker/).

## Use the data

| File | What is inside |
|---|---|
| [`data/caption-limits.json`](data/caption-limits.json) | Max characters, counting method, fold, hashtag cap per network |
| [`data/image-sizes.json`](data/image-sizes.json) | Width, height, ratio, safe zone and note per format |
| [`data/safe-zones.json`](data/safe-zones.json) | Margins in pixels and the safe area for 9:16 formats, with sources |

```js
const limits = await fetch("https://raw.githubusercontent.com/Mydrop-AI/social-media-specs/main/data/caption-limits.json").then((r) => r.json());
limits.find((l) => l.network === "x").maxCharacters; // 280
```

Counting methods in `caption-limits.json`:

- `default`: Unicode code points (an emoji counts as 1)
- `utf16`: UTF-16 code units (an emoji or a CJK character counts as 2)
- `x`: Weighted: CJK and most emoji count as 2, any link counts as 23

## Something changed?

Networks change their specs often. Open an issue or a pull request with a link to the network's own documentation, and we update the table and the free tools together.

## License

MIT. Use the data anywhere; a link back to [mydropai.com](https://mydropai.com/) is welcome.
