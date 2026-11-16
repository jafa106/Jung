# Carl Jung, in his own words

A self-contained, installable web app that runs **semantic search over Carl Jung's own words**
entirely in your browser — no server. Type a question and get back his most relevant passages
from four public-domain primary works (Psychology of the Unconscious, Collected Papers on
Analytical Psychology, The Theory of Psychoanalysis, Psychological Types — 6,240 passages).

- **Engine:** [transformers.js](https://github.com/xenova/transformers.js) `all-MiniLM-L6-v2`,
  embeddings computed on first load and cached in IndexedDB; top-8 cosine similarity.
- **Offline-capable PWA:** installable via *Add to Home Screen*; works offline after first visit.

> Note: first load embeds the corpus in-browser (a few minutes), then it's cached permanently.

## Run locally
```
python3 -m http.server 8080
# open http://localhost:8080
```

## Live site
GitHub Pages → https://jafa106.github.io/Jung/

*Texts are public-domain English editions (1915–1923) from Project Gutenberg and the Internet
Archive. Jung's later, copyrighted work is not included.*
