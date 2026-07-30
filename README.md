# contrast-checker

A WCAG color contrast ratio checker. Pick a text color and a background
color (native color pickers plus hex text fields) and get a live
contrast ratio, pass/fail results for WCAG AA and AAA at both normal and
large text sizes, and a live text preview so the effect is visible, not
just the number.

Live: https://sidcore-dev.github.io/contrast-checker/

## Why

WCAG 2.1 sets minimum contrast ratios for readable text (4.5:1 for AA
normal text, 3:1 for AA large text, 7:1 for AAA normal text, 4.5:1 for
AAA large text), but eyeballing whether a color pair clears those bars
is unreliable. This tool computes the ratio directly from the WCAG
relative-luminance formula and shows the result immediately.

## Static, client-side tool

This is a single self-contained `index.html` file — no build step, no
server, no external scripts or fonts. Everything (markup, styles,
JavaScript) lives in that one file and runs entirely in your browser;
no color values are ever sent anywhere. You can open `index.html`
directly from disk, or use the hosted version above.

## License

All rights reserved. This code is public for viewing and reference only —
no license is granted to use, copy, modify, or redistribute it. See
[LICENSE](LICENSE) for details.
