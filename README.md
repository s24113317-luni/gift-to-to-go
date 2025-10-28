# gift-to-to-go

A lightweight single-file demo: "Gift-on-the-Go Vending Machine" (index.html).

Features added by enhancement:

- Original: choose gift type, box style, enter message, Create Gift (keeps original behavior).
- Security: user input is HTML-escaped before inserting into the output to prevent XSS.
- Accessibility: `aria-live` on the output, improved focus outlines for keyboard users.
- Extras (non-invasive additions):
  - Confetti canvas animation and sound when creating a gift.
  - Extra controls: Surprise, Save, Share, Copy, Download, Theme toggle.
  - Preview and price breakdown panels.
  - Keyboard shortcuts: `S` for Surprise, `Ctrl/Cmd+Enter` to Create.
  - Persisted preferences: last message and theme stored in localStorage.

How to use:

1. Open `index.html` in your browser.
2. Choose gift options and click "Create Gift".
3. Use "Surprise Me" to auto-fill and create; use Download/Copy/Share to export the summary.
4. Toggle Theme to switch to a calmer light theme; the choice is saved.

Notes and caveats:

- The enhancements are non-destructive; the original `generateGift()` behavior is preserved.
- For full security, consider rendering output via DOM methods instead of template strings.

Author: s24113317-luni
License: MIT
