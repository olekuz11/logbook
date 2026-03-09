# logbook

field notes. progress. sounds. things noticed.

→ [olekuz11.github.io/logbook](https://olekuz11.github.io/logbook)

---

## how to add an entry

open `index.html`. paste this block at the **top** of `<main>`, just after the comment:

```html

  
    YYYY-MM-DD
    TAGNAME
  
  
    your text here.
  

```

**tags:** `progress` / `reading` / `listening` / `watching` / `sonic` / `thinking`

---

## how to add a sonic entry

1. record on phone → save as `.ogg` or `.mp3`
2. rename: `tape_NNN_location_detail.ogg` (e.g. `tape_004_bus_rain.ogg`)
3. drop the file into `sounds/`
4. add entry to `index.html` with `data-tag="sonic"` and an `<audio>` element:

```html

  
    YYYY-MM-DD
    sonic
  
  
    brief note on what it is.
    
      tape_NNN — description
      
        
      
    
  

```

sonic entries appear in both the main log and automatically in `sound.html`.

---

## file structure

```
logbook/
├── index.html     ← the log (edit this to add entries)
├── sound.html     ← sonic diary (auto-populated)
├── style.css      ← all styles
├── README.md
└── sounds/        ← drop .ogg / .mp3 files here
```

---

*code as if nobody's watching.*