A repository for golden image files that are used by tests that for whatever reason can't use the Skia Gold testing infrastructure.

## Getting diffs for golden images

If you have ImageMagick and you want to use it to show diffs of files
in this repo, add the following to your `~/.gitconfig`:

```
[diff "image"]
    command = /path/to/this/repo/diff-images.sh
```
