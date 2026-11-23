# Document Search

A single web page that searches inside your Word (.docx) and text files. Open it, choose files or a whole folder,
and type a query: every place a match shows up is listed, and clicking one opens the document in the page at that
spot.

**Nothing leaves your browser.** The files are read by the browser itself, in memory. The page has no server side,
loads nothing from anywhere else, and its Content-Security-Policy forbids network connections, so it could not send
your files anywhere even if it tried. Nothing is stored; closing the tab forgets everything.

Search syntax: `budget report` (both words), `"next quarter"` (phrase), `analy*` and `gr?y` (wildcards), `+must`,
`-draft`, `invoice OR receipt`, `file:*.docx` (by file name), `/regex/`. Options for whole words, match case, any/all
words, and same-file or same-paragraph matching.

Everything is in `index.html`; save it and it works offline from your disk too.
