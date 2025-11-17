#  Data management
- **Always backup** your data (with an external HD or via the internal Lina system).
- **Do not rely on Discord as long-term storage.**

## Raw data and processed results
- Use the appropriate NAS for raw data and processed results.
- Always separate raw data and processed results.
- Use the following tree structures:
```
data/
├── project/
│   ├── YYYY/
│   │   └── YYYY-MM-DD/
│   │       └── YYYY-MM-DD-short-description-or-experimental-parameters.raw
│   │       └── README.md
```
```
proc/
├── project/
│   ├── YYYY/
│   │   └── YYYY-MM-DD-short-title/
│   │       └── figure-1.png
│   │       └── script.py
│   │       └── notebook.ipynb
│   │       └── README.md
```
-  To avoid data spreading, a `project` folder should be broad enough (e.g. a topic like `two-pp` or `dlw`).
- The exact file name can be a bit flexible but i) always use the correct date format and ii) always keep track of the data description in your labbook (paper and digital format).
- Add a README file if needed.

## Reports and presentation
- Use our shared OneDrive for regular file sharing (reports, presentations, figures, labbook, etc.).
- Use date formatted file names: `YYYY-MM-DD-my-presentation.ppt`

## Labbook
- Use our shared `labnotes` OneDrive folder as digital labbook.