## Problem

re-frame docs are everywhere. I just want to search for a specific keyword and find all the relevant literature.

## Solution

Concatenate all the `.md` files in re-frame docs to one document that is searchable, PDFable, etc.

Quick and dirty:

```
for i in $(ls docs/); do cat docs/$i >> re-frame-one-doc.md; done
for i in $(ls docs/FAQs/); do cat docs/FAQs/$i >> re-frame-one-doc.md; done
```

Last compiled on August 10th, 2017. No order or anything, just `ctrl-f` it.

All docs taken from https://github.com/Day8/re-frame
