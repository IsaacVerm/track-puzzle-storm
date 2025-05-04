# Track Puzzle Storm

Make sure [Datasette is serving puzzles.db](https://github.com/IsaacVerm/puzzle-storm-extension/blob/main/doc/how-to-run-extension.md) so we can fetch the puzzles. Run this in the `puzzle-storm-extension` repo:

```bash
datasette puzzles.db
```

Now update `puzzles.csv`:

```bash
curl -o puzzles.csv "http://127.0.0.1:8001/puzzles/puzzles.csv?_sort_desc=timestamp&_size=max"
```