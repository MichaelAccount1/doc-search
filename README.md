# Document Search

A single web page that searches inside your Word (.docx) and text files. Open it, choose files or a whole folder,
and type a query: every place a match shows up is listed, and clicking one opens the document in the page at that
spot.

**Your files stay in your browser.** They are read by the browser itself, in memory: the page doesn't upload them or
save them anywhere, loads nothing from elsewhere, and its Content-Security-Policy forbids it from making network
connections. Closing the tab forgets everything. (The copy buttons use your clipboard.)

In Word files it searches the body, tables, text boxes, headers, footers, footnotes, endnotes and comments.

Search syntax: `budget report` (both words), `"next quarter"` (phrase), `analy*` and `gr?y` (wildcards), `+must`,
`-draft`, `invoice OR receipt`, `file:*.docx` (by file name), `/regex/`. Options for whole words, match case, any/all
words, and same-file or same-paragraph matching.

Everything is in `index.html`; save it and it works offline from your disk too.
