# logbook

personal HTML field notes. progress. sounds. things noticed.

→ [olekuz11.github.io/logbook](https://olekuz11.github.io/logbook)

---

## how to add an entry

open `index.html`. paste this block at the **top** of `<main>`, just after the comment:
```html
<article class="entry" data-tag="TAGNAME">
  <div class="entry-meta">
    <time class="entry-date">YYYY-MM-DD</time>
    <span class="entry-tag TAGNAME">TAGNAME</span>
  </div>
  <div class="entry-body">
    <p>your text here.</p>
  </div>
</article>
```

**tags:** `progress` / `reading` / `listening` / `watching` / `sonic` / `thinking`

---

## how to add a sonic entry

1. record on phone — use hyphens not spaces in filename (e.g. `tape_002_midnight-kitchen.m4a`)
2. upload to **archive.org/upload** — add to existing item or create one dedicated item for the whole diary
3. get the stable direct URL from the download section:
   `https://archive.org/download/ITEM-IDENTIFIER/filename.m4a`
4. add entry to `index.html` with `data-tag="sonic"` and an `<audio>` element (see below)

sonic entries appear in both the main log and automatically in `sound.html`.

---

## file structure
```
logbook/
├── index.html     ← the log (edit this to add entries)
├── sound.html     ← sonic diary (auto-populated)
├── style.css      ← all styles
└── README.md
```

audio files are hosted on archive.org — not stored in this repo.

---

*code as if nobody's watching.*
```

