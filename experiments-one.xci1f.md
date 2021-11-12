---
id: xci1f
date: 2021-11-11 21:18:06-0700
title: "Experiments One"
---

## Experiment One: Which formats are detected and which resolve correctly?

### These aren't detected as links at all (no LSP hints at all)

[[ker6z|these terms]]
[[.ker6z|these terms]]
[[ker6z.|foo]]
[[terms-of-gardening | these terms]]

### These get detected as a link, but result in 'not found' LSP indicators

[[ker6z | these terms]]
[[.ker6z | these terms]]
[[ker6z. | foo]]
[[Digital Garden/terms-of-gardening.ker6z | these terms]]
[[Digital Garden/terms-of-gardening.ker6z.md | these terms]]

[Terms of Gardening](terms-of-gardening.ker6z)
[Terms of Gardening](ker6z)

#### These get detected as links and result in not found, but that's expected

Flipping the Wiki link syntax around (putting the label on the left of the `|`
character) does not affect the parsing.

[[these terms | Digital Garden/terms-of-gardening.ker6z]]
[[these terms | terms-of-gardening]]
[[these terms | Digital Garden/terms-of-gardening.ker6z.md]]
[[these terms|ker6z]]
[[these terms | ker6z]]

### These work as expected

[[Terms of Gardening]]
[[Digital Garden/terms-of-gardening.ker6z]]
[[Digital Garden/terms-of-gardening.ker6z.md]]
[[terms-of-gardening]]
[[.ker6z]]
[[ker6z]]
[[ker6z.]]

[Terms of Gardening](Digital%20Garden/terms-of-gardening.ker6z)
[Terms of Gardening](Digital Garden/terms-of-gardening.ker6z)
