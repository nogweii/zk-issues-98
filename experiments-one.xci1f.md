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
[[these terms|ker6z]]
[[these terms | ker6z]]
[[.ker6z | these terms]]
[[ker6z. | foo]]
[[these terms | Digital Garden/terms-of-gardening.ker6z]]
[[Digital Garden/terms-of-gardening.ker6z | these terms]]
[[these terms | terms-of-gardening]]
[[Digital Garden/terms-of-gardening.ker6z.md | these terms]]
[[these terms | Digital Garden/terms-of-gardening.ker6z.md]]

[Terms of Gardening](terms-of-gardening.ker6z)
[Terms of Gardening](ker6z)

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
