# CSS defaults

A collection of stylesheets that I like to build on.

## Stylesheets

There is a hierarchy between the stylesheets.
Higher-level sheets may not contain rules that are already covered by lower-level sheets.
However, the goal is that each stylesheet forms a logical group of CSS rules that can stand on its own.

### `reset.css`

A stylesheet to set sane defaults, reduce browser inconsistencies and improve user and developer experiences based on the following resources:

- Base rule set: Josh W. Comeau's [A Modern CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/).
    - Without creating a root stacking context.
- Adjustments inspired by [Notes on Josh Comeau’s Custom CSS Reset](https://css-tricks.com/notes-on-josh-comeaus-custom-css-reset):
    - Remove all padding. Add padding to lists to respect list items markers.
    - Make `iframe` and `object` block elements like other media elements.
    - Additionally avoid text overflow for `li`, `dt`, `dd`, and `blockquote` elements.
    - Move global typography sizing rules to the `html` selector.
- Prevent font size inflation: [Your CSS reset needs text-size-adjust (probably)](https://kilianvalkhof.com/2022/css-html/your-css-reset-needs-text-size-adjust-probably/).
    - With caring about vendor prefixes.

### `typography.css`

A stylesheet with typography related rules. Provides different system font stacks[^1] to choose from.

- System font stacks from the following sources are provided:
    - [Tailwind CSS](https://tailwindcss.com/docs/font-family),
    - [Bootstrap](https://getbootstrap.com/docs/5.0/content/reboot/#native-font-stack),
    - [Modern Font Stacks](https://github.com/system-fonts/modern-font-stacks), and
    - [GitHub](https://github.com/) (inspect the page with your browser's developer tools).
- Font stacks are assigned appropriately.
- Typography related rules of [modern-normalize](https://github.com/sindresorhus/modern-normalize).

[^1]: A system font stack relies on the fonts of the operating system, such that, among other advantages, no font hast to be downloaded.

## Licence

Distributed under the [MIT](https://spdx.org/licenses/MIT.html) licence. See [LICENSE.md](./LICENSE.md) for more information.
