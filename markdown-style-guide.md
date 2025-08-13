# Markdown Style Guide (Short & Simple)

This guide shows how to write clean, easy-to-read Markdown for documents, reports, and technical notes.  
Examples show **good** ✅ and **bad** ❌ usage.


## 1. Minimum Documentation
- Keep only what’s **useful and up to date**.
- Delete old or unused docs.
- Better to have a few good docs than many bad ones.


## 2. Capitalization
- Keep original product/tool names as they are.
  - ✅ `Markdown`  
  - ❌ `markdown`


## 3. Document Layout
Start with:
```markdown
# Document Title

Short 1–3 sentence introduction.

[TOC]   <!-- If supported, generates Table of Contents -->

## First Topic

Your content here.

## See Also

* https://link-to-more-info
```
- Only **one** `#` heading per doc (the title).
- Rest should be `##` or smaller.


## 4. Table of Contents
- Use `[TOC]` **after the introduction**.
- Not needed if the doc is very short.


## 5. Line Length
- Limit text lines to **~80 characters** (code style).
- Exception: links, tables, and code blocks.


## 6. Headings
- Use **ATX style** (`#`, `##`, etc.).
- Leave a blank line before/after headings.
- Make headings **clear and unique**.

✅  
```markdown
## Connecting to the Database
```

❌  
```markdown
## Heading 2
```


## 7. Lists
- Use **lazy numbering** for long lists:

  1.  Step one
  1.  Step two
  1.  Step three
- For nested lists, indent **4 spaces**.



## 8. Code
### Inline Code
- Wrap short code in backticks:
  ```markdown
  Run `my_script.sh` to start.
  ```

### Code Blocks
  - Use triple backticks and **declare the language**:
    ```python
    def greet(name):
        print(f"Hello {name}")
    ```
- Use fenced code blocks (` ``` `), not indented ones.
- Inside lists, indent the code block.



## 9. Links
### Short Links Inline
```markdown
Read the [Markdown Guide](markdown.md).
```

### Long or Repeated Links → Reference Style
```markdown
See the [style guide][style].

[style]: https://example.com/style-guide
```



## 10. Images
```markdown
![Alt text for screen readers](image.png)
```
- Keep images simple.
- Always write **alt text**.



## 11. Tables
✅ Use when data fits well in rows/columns:
```markdown
| Tool     | Purpose        |
|----------|----------------|
| Git      | Version control|
| Markdown | Documentation  |
```
| Tool     | Purpose        |
|----------|----------------|
| Git      | Version control|
| Markdown | Documentation  |

❌ Don’t use tables for long text → use lists instead.



## 12. Avoid HTML
- Use Markdown syntax whenever possible.
- HTML reduces readability and tool compatibility.




**Quick Reminder:**
- Keep docs **clear and simple**.
- Delete what’s outdated.
- Format headings, lists, code, links consistently.
- Write for **future readers**, not just yourself.




**Reference:**  
This style guide is adapted and shortened from the [Google Markdown Style Guide][g-style].

[g-style]: https://google.github.io/styleguide/docguide/style.html#minimum-viable-documentation
