#  Data management
!!! warning 
    - **Always backup** your data (with an external HD or via the internal Lina system).
    - **Do not rely on Discord as long-term storage.**

## Raw data and processed results
- Use the appropriate NAS for raw data and processed results.
- Always separate raw data and processed results.

### Naming convention
Use the following tree structures:
```
data/
├── project/
│   ├── YYYY/
│   │   └── YYYY-MM-DD/
│   │       └── YYYY-MM-DD_short-description-or-experimental-parameters.raw
│   │       └── README.md
```
```
proc/
├── project/
│   ├── YYYY/
│   │   └── YYYY-MM-DD_short-title/
│   │       └── figure-1.png
│   │       └── script.py
│   │       └── notebook.ipynb
│   │       └── README.md
```

!!! note
    - To avoid data spreading, a `project` folder should be broad enough (e.g. a topic like `two-pp` or `dlw`).
    - Keep track of the data description in your labbook (paper **and** digital format).
    - Add a README file if needed to add explanations.

## Regular file sharing
Use our shared sDrive for regular file sharing (reports, presentations, figures, lab notes, etc.).

### Naming convention
Use these rules for **all** files and folders.

1. **Use ISO dates (YYYY-MM-DD)**

    Examples:  
    `2025-03-12_scan-1.dat`  
    `2025-11-08_experiment-notes.md`

2. **No spaces — use hyphens or underscores**

    Good: `temp_sweep_2025-02-01.csv`  
    Bad: `temp sweep.csv`

3. **Most specific information first**

    `YYYY-MM-DD_topic_details.ext`
    Example: `2025-03-12_raman_sample-A.csv`

4. **Versioning**
    
    Use Git for code and textual content. For other files, use:  
    `v1`, `v2`, `v3`, etc. or date-based versions.

    Example:
    `manuscript_v3.docx`  
    `2025-04-10_analysis-v2.ipynb`

## Lab notes
- Use our shared `labnotes` sDrive folder as digital labbook.
- Lab notes are written in Markdown and are organized by **year/month**. 
- Notes include **metadata for indexing and search**.

### Folder and file naming

### Naming convention

#### Tree structure
```
labnotes/
├── notes/
│   ├── 1849/
│   │   └── 09/
│   │       └── 1849-09-23_HF.md  # Hippolyte Fizeau
│   ├── 1881/
│   │   │── 01/
│   │       └── 1881-01-01_AAM.md  # Albert A. Michelson
│   ├── 1887/
│   │   └── 12/
│   │       └── 1887-12-19_AAM.md
│   ├── 1960/
│   │   │── 01/
│   │       └── 1960-01-11_TM.md  # Theodore Maiman
│   │   │── 05/
│   │       └── 1960-05-16_TM.md
│   ├── assets/
│   │   │── img/
│           └── 1960-05-16_TM-laser.png
└── labindex.py
└── README.md
```

#### File format
```
YYYY-MM-DD_<YourInitials>.md
```

### Note template
```markdown
---
date: YYYY-MM-DD
author: Firstname Lastname
title: Short title
tags: tag1, tag2
---

Write your content here using Markdown.

Put images in `../../assets/img` following the file naming.

![](../../assets/img/YYYY-MM-DD_<YourInitials>-<short description>.png)
```

### Generating the index

Run this command in the Terminal to regenerate `index.html`:
```bash
python labindex.py
```
### Usage

- Edit notes using the [Markdown format](https://www.markdownguide.org/basic-syntax/)
- Save notes in the correct `YYYY/MM/` folder
- File name must follow `YYYY-MM-DD_<YourInitials>.md`
- Regenerate the index after adding or updating notes
- Search in the index by tags or any text
    * For tags, `OR` = comma or space separated and `AND` = plus-separated 
    * Search examples:
```
author:Fizeau; tags:interferometer+light
tags:laser,light 
author:Michelson; year:1887
```