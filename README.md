# Before / After Slider

A small image comparison slider for embedding in Notion case studies. A line follows the cursor and reveals the left or right image.

## Make an embed

1. Add your screens to the `images/` folder and push.
2. Build the link (replace the file names and labels):

   ```
   https://elliotchev.github.io/before-after-slider/?a=images/before.png&b=images/after.png&la=Before&lb=After
   ```

   | Param | What it sets |
   |-------|--------------|
   | `a`   | Left image (path in this repo or any public image URL) |
   | `b`   | Right image |
   | `la`  | Left label (default "Before"; leave empty to hide) |
   | `lb`  | Right label (default "After") |

3. In Notion, type `/embed` and paste the link.

Opening the page without `a` and `b` shows the editor, where you can preview images, rename labels and copy a link.

## Images that always load

- Keep screens in `images/` in this repo. Relative paths like `images/x.png` load from GitHub Pages for every visitor.
- File names are case-sensitive on GitHub Pages: `Checkout.PNG` is not `checkout.png`.
- Avoid spaces in file names, or write them as `%20` in the link.
- Don't use links copied from Notion images. They expire after about an hour.
- Uploads in the editor stay in your browser only, so they never appear in an embed.
- Export at 2x and compress (WebP or optimised PNG) so embeds load fast.
