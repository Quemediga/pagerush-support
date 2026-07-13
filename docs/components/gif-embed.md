# Component: GifEmbed

## Purpose
Displays an animated GIF from an uploaded PageRush/Firebase image URL or from giphy.com.

## When to Use
* Showing short animations or screen recordings.
* Adding visual interest or humor (use sparingly!).
* Illustrating a quick process visually.

## How to Use (Options / Props)

| Option (`prop`) | Description                                      | Required? | Example Value(s)                     |
| :-------------- | :----------------------------------------------- | :-------- | :----------------------------------- |
| `src`           | An uploaded GIF URL from PageRush/Firebase Storage or a giphy.com GIF URL. | Yes | `"https://firebasestorage.googleapis.com/..."`, `"https://i.giphy.com/media/.../giphy.gif"` |
| `alt`           | Text description of the GIF for accessibility. | Yes       | `"Animation showing button click"` |
| `caption`       | Optional text displayed below the GIF.           | No        | `"Fig. 1: Saving the file."`       |

## Example MDX Usage

**Uploaded GIF:**
```mdx
<GifEmbed
  src="https://firebasestorage.googleapis.com/v0/b/sites-carlosalegre-com-d7113.firebasestorage.app/o/Images%2Fdemo.gif?alt=media"
  alt="Loading animation spinner"
/>
```

**Giphy GIF with a Caption:**
```mdx
<GifEmbed
  src="https://i.giphy.com/media/bF3y2QS0U0sdgtz8sZ/giphy.gif"
  alt="Short demo showing the new feature in action"
  caption="Quick look at the drag-and-drop interface."
/>
```
