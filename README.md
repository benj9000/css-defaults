# CSS defaults

A collection of CSS rules that I like to build on.

## Sources

- Base rule set: Josh W. Comeau's [A Modern CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/).
    - Without creating a root stacking context.
- Adjustments inspired by [Notes on Josh Comeau’s Custom CSS Reset](https://css-tricks.com/notes-on-josh-comeaus-custom-css-reset):
    - Remove all padding. Add padding to lists to respect list items markers.
    - Make `iframe` and `object` block elements like other media elements.
    - Additionally avoid text overflow for `li`, `dt`, `dd`, and `blockquote` elements.
    - Move global typography sizing rules to the `html` selector.

## Licence

Distributed under the [MIT](https://spdx.org/licenses/MIT.html) licence. See [LICENSE.md](./LICENSE.md) for more information.
