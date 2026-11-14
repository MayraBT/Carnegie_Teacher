# Carnegie TEKS Lookup for Teachers · Dallas ISD Math

The teacher and campus version of the coordinators' Carnegie TEKS Lookup (`MayraBT/Carnegie_DOT_CHART`), 6th Grade Advanced through Algebra II Advanced.

**What's in it:** each Carnegie lesson with its TEKS dots from the Carnegie dot charts (and, for 7th Advanced, the TEKS listed on the IPC) and its Teacher Implementation Guide link; By standard (student expectation, vocabulary, vertical alignment, released STAAR items with Texas percents); Teaching moves; and the Full grid.

**Left out on purpose:** IPC pacing and calendars (no Calendar view, no dates, no "Taught in" quarter filters), Dallas ISD STAAR results, and the ACP Example items for Geometry and Algebra II (district-secured).

Teaching moves are suggestions, not a complete list, and not a checklist for evaluating teacher instruction or performance.

## Updating
This page is generated from the coordinator version. After any change there:

```
python3 build/teacherize.py ../Carnegie_DOT_CHART/index.html index.html carnegie
mkdir -p items && cp ../Carnegie_DOT_CHART/items/g* items/   # never copy items/acp_*
```
Then test (`build/test_teacher.js`, with a local server on port 8770 serving the parent folder) and push.

Sources: lead4ward IQ Tool (released STAAR items and Texas percents), lead4ward TEKS Scaffold and Academic Vocabulary, 19 TAC §111 (TEKS), Carnegie Learning Texas Math Solution TEKS dot charts (lesson TEKS).
