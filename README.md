# Track Puzzle Storm

Make sure the [puzzles Flask app is running](https://github.com/IsaacVerm/puzzle-storm-extension/blob/main/doc/how-to-run-extension.md) so we can fetch the puzzles.

With the API running:

```bash
curl -o puzzles.csv "http://127.0.0.1:8001/puzzles/puzzles.csv?_sort_desc=timestamp&_size=max"
```