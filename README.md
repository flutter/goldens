A repository for golden image files that are used by tests in https://github.com/flutter/flutter.

See: https://github.com/flutter/flutter/wiki/Writing-a-golden-file-test-for-package%3Aflutter

## Getting diffs for golden images

If you have ImageMagick and you want to use it to show diffs of files
in this repo, add the following to your `~/.gitconfig`:

```
[diff "image"]
    command = /path/to/this/repo/diff-images.sh
```

## Obsolete files

To make it easier to land multiple PRs that change the goldens in
parallel, when you change the result of a test, rather than just
updating the golden file, rename the golden file so that after your
change we use a different image than before your change, and then
update the list of obsolete images here to include the old name:

- packages/flutter/test/material/floating_action_button_test.clip.1.png
