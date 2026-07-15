# Citation Values Activity 2

An interactive, self-contained learning activity for an open-source module on citations. Learners match citation conventions to the relationships and responsibilities they support, then check their answers against an answer key.

## What it does

A matrix pairs each **citation convention** with its **corresponding academic or social value**. Learners tick checkboxes across three columns:

- Relationship with past knowledge producers
- Relationship with future knowledge producers
- Responsibilities to ourselves as writers

Clicking **Check answers** grades every cell. A cell counts as correct when its checked/unchecked state matches the key, so learners are rewarded both for checking the right boxes and for correctly leaving others empty. Correct cells turn green and read "Correct"; mismatches turn pink and read "Try again!". **Reset** clears all selections.

## Usage

No build step, no dependencies. Everything (HTML, CSS, JavaScript) lives in a single `index.html`.

- **Open locally:** double-click `index.html`, or open it in any browser.
- **Embed in a module:** drop `index.html` into your course files, or embed it in an `<iframe>`.

## Hosting on GitHub Pages

1. Push this repository to GitHub.
2. Go to **Settings → Pages**.
3. Under **Build and deployment**, set **Source** to *Deploy from a branch*, pick your default branch and the `/ (root)` folder, and save.
4. Your activity will be live at `https://<your-username>.github.io/<repo-name>/`.

## Editing the content

The activity content and answer key live in the `ROWS` array near the top of the `<script>` block in `index.html`. Each entry has:

```js
{
  convention: "…",        // left column text
  value: "…",             // second column text
  key: [past, future, self] // true = box should be checked
}
```

Change the text or flip a `true`/`false` to adjust the answer key. No other files need editing.
