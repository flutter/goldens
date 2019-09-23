A repository for golden image files that are used by tests in https://github.com/flutter/flutter.

See: https://github.com/flutter/flutter/wiki/Writing-a-golden-file-test-for-package%3Aflutter

PLEASE READ THAT WIKI PAGE BEFORE CONTRIBUTING TO THIS REPOSITORY.

IT CONTAINS RULES THAT YOU MUST FOLLOW.

## Getting diffs for golden images

If you have ImageMagick and you want to use it to show diffs of files
in this repo, add the following to your `~/.gitconfig`:

```
[diff "image"]
    command = /path/to/this/repo/diff-images.sh
```

## Obsolete files

To make it easier to land multiple PRs that change the goldens in
parallel, when we change the result of a test, rather than just
updating the golden file, we change the name of the golden file
used in the test, so that after the change we use a different
image than before the change.

This section lists the files that can now be deleted because
they have been replaced in this way:

- packages/flutter/test/cupertino/switch.tap.off.0.png
- packages/flutter/test/cupertino/switch.tap.on.0.png
- packages/flutter/test/cupertino/switch.tap.turningOn.0.png
- packages/flutter/test/cupertino/date_picker_test.datetime.drag.1.png
- packages/flutter/test/cupertino/date_picker_test.datetime.initial.1.png
- packages/flutter/test/cupertino/date_picker_test.datetime.drag.png
- packages/flutter/test/cupertino/date_picker_test.datetime.initial.png
- packages/flutter/test/cupertino/text_field_cursor_test.0.0.png
- packages/flutter/test/cupertino/text_field_cursor_test.1.0.png
- packages/flutter/test/cupertino/text_field_cursor_test.0.1.png
- packages/flutter/test/cupertino/text_field_cursor_test.1.1.png
- packages/flutter/test/cupertino/text_field_cursor_test.0.2.png
- packages/flutter/test/cupertino/text_field_cursor_test.1.2.png
- material/bottom_navigation_bar.shifting_transition.2.0.png
- material/bottom_navigation_bar.shifting_transition.2.1.png
- material/bottom_navigation_bar.shifting_transition.2.3.png
- material/bottom_navigation_bar.shifting_transition.2.4.png
- material/bottom_navigation_bar.shifting_transition.2.5.png
- material/bottom_navigation_bar.shifting_transition.2.6.png
- material/bottom_navigation_bar.shifting_transition.2.7.png
- packages/flutter/test/material/text_field_cursor_test.0.0.png
- packages/flutter/test/material/text_field_cursor_test.1.0.png
- packages/flutter/test/material/text_field_opacity_test.0.2.png
- packages/flutter/test/material/floating_action_button_test.clip.1.png
- packages/flutter/test/widgets/editable_text_test.0.2.png
- packages/flutter/test/widgets/editable_text_test.1.2.png
- packages/flutter/test/widgets/editable_text_test.0.1.png
- packages/flutter/test/widgets/editable_text_test.1.1.png
- packages/flutter/test/widgets/editable_text_test.0.0.png
- packages/flutter/test/widgets/editable_text_test.1.0.png
- packages/flutter/test/widgets/text_golden.DecorationThickness.1.0.png
- packages/flutter/test/widgets/text_golden.TextInlineWidget.2.1.png
- packages/flutter/test/widgets/text_golden.TextInlineWidgetNest.1.1.png
- packages/flutter/test/widgets/text_golden.TextInlineWidget.1.0.png
- packages/flutter/test/widgets/text_golden.TextInlineWidgetBaseline.1.0.png
- packages/flutter/test/widgets/text_golden.TextInlineWidgetAboveBaseline.1.0.png
- packages/flutter/test/widgets/text_golden.TextInlineWidgetBelowBaseline.1.0.png
- packages/flutter/test/widgets/text_golden.TextInlineWidgetTop.1.0.png
- packages/flutter/test/widgets/text_golden.TextInlineWidgetMiddle.1.0.png
