# NHEB text by chapter

The **New Heart English Bible**, edited by Wayne A. Mitchell, **Update June 4, 2026**, split into one plain-text file per chapter.

## Source

- Official plain-text edition: https://nheb.net/files/NHEB.txt
- SHA-256 of the pinned copy these files were built from (LF line endings): `b3977af667cf1fef7dcc9fd1e6738df891ae20252025a348e0714b42a3aa94d3`
- nheb.net serves the same text with CRLF line endings, SHA-256 `51b6744ad1c464328850e0d7277f48af77324d0966d9dcee7a2c7e984f52799a`.
- 31,102 verses, 1,189 chapters, 66 books.

Notice from the source file's header:

> New Heart English Bible, in text format. Edited by Wayne A. Mitchell
> Public Domain 2007-2026 (Update June 4, 2026).

## Layout

- `<Book code>/<chapter>.txt`: one verse per line, `Code Chapter:Verse text`, each line exactly as in the source file (UTF-8, LF line endings, no byte-order mark). Two verses (1Ki 15:5 and 15:7) separate the reference from the text with a narrow no-break space (U+202F), as published.
- [BOOKS.md](BOOKS.md): the three-letter book codes and full book names, in canonical order.

## Fetching a chapter

```
https://raw.githubusercontent.com/DELministries/nheb-text/main/<Book code>/<chapter>.txt
```

For example, John 3: https://raw.githubusercontent.com/DELministries/nheb-text/main/Joh/3.txt

These files are generated from the source file by a script; they are not edited by hand. A new edition replaces them in one commit naming the edition and the source hash.
