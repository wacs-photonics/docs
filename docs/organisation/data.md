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
- Use our shared sDrive for regular file sharing (reports, presentations, figures, lab notes, etc.).
- Please use the following **naming conventions**. Use these rules for **all** files and folders.

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

## Labbook
- Use our shared `labnotes` sDrive folder as digital labbook.