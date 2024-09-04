# collapser.js

`collapser.js` is a tiny JavaScript library for automatically collapsable
headings (or arbitrary nodes)

## Usage

1. Add `collapser.js` to your website
2. Add the class `"collapser"` to any heading (or other node) that should be
   able to collapse it's content
3. Add the class `"collapser-init-show"` to any collapser whose content should
   be visible by default (and not hidden by default)

The collapsables content is always its `nextElementSibling` and its visibility
is toggled between `"block"` and `"none"`. If the node has more than one semantic
child, consider wrapping them all in a `span` or `div`.

## Customization

The following variables can be used to customize `collapser.js`. They can
either be edited at the top of the script (globally) or be set by a different
script before loading it (locally). The list shows the default value.

- `collapserClassName := "collapser"` (class name of collapser nodes)
- `collapserInitShowClassName := "collapser-init-show"` (class name for
  collapsers that are active by default)
- `collapserActivePrefix := "&blacktriangledown;"` (string that is prefixed to
  the collapser's innerHTML when its content is shown)
- `collapserInactivePrefix := "&blacktriangleright;"` (string that is prefixed
  to the collapser's innerHTML when its content is hidden)
- `collapserDisplayShow := "block"` (value for content's display when shown)
- `collapserDisplayHide := "none"` (value for content's display when hidden)

Note that if any of the values are supposed to be have false-ish value (e. g.
empty string) changing it locally by pre-defining it won't work.

## License

This was such a miniscule amount of work and is also the canonical solution so
the license is »whatever«. Do with the code _whatever_ you please.
