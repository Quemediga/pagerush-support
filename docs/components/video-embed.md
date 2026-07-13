# Component: VideoEmbed

## Purpose
Easily embeds a video player from YouTube or Vimeo into your content.

## When to Use
* Showing product demos.
* Including tutorials or walkthroughs.
* Embedding webinars or presentations.

## How to Use (Options / Props)

| Option (`prop`) | Description                                               | Required? | Example Value(s)                  |
| :-------------- | :-------------------------------------------------------- | :-------- | :-------------------------------- |
| `src`           | The full URL of the YouTube or Vimeo video.              | Yes       | `"https://www.youtube.com/watch?v=..."`, `"https://vimeo.com/..."` |
| `title`         | A description of the video for accessibility.             | Yes       | `"Product Demo Video"`, `"Tutorial on X"` |

## Example MDX Usage

**Embedding a YouTube Video:**
```mdx
<VideoEmbed
  src="https://www.youtube.com/watch?v=dQw4w9WgXcQ"
  title="Example YouTube Video"
/>
```

**Embedding a Vimeo Video:**
```mdx
<VideoEmbed
  src="https://vimeo.com/123456789"
  title="Example Vimeo Video Showcase"
/>
```
