# Open Design #8895 export evidence

The same benign project fixture was exported through the production `inlineRelativeAssets` function at
[baseline `93d4031`](https://github.com/nexu-io/open-design/commit/93d4031572df0ab05307558eb8d8486cdc4c287c)
and [PR head `c18441d`](https://github.com/nexu-io/open-design/commit/c18441d343b93020a5c81ae14fd5b72f9c334459).
`before.html` and `after.html` are the emitted HTML bytes.

Serve the directory with `python3 -m http.server 8000` and open http://localhost:8000 to see the browser results side by side.
The fixture uses entity-encoded relative CSS/JS filenames and a stylesheet title/media control.
This comparison exercises the inliner and its emitted HTML. The PR separately contains the HTTP export-route regression.
