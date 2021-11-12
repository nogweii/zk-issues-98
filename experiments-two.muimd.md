---
id: muimd
date: 2021-11-11 21:18:50-0700
title: "Experiments Two"
---

## Experiment Two: Does the space in the folder name matter?

### These aren't detected as links at all (no LSP hints at all)

[[1kfxj|these terms]]
[[.1kfxj|these terms]]
[[1kfxj.|foo]]

### These get detected as a link, but result in 'not found' LSP indicators

[[1kfxj | these terms]]
[[.1kfxj | these terms]]
[[1kfxj. | foo]]
[[Digital-Garden/gardening-terms.1kfxj | these terms]]
[[Digital-Garden/gardening-terms.1kfxj.md | these terms]]
[[gardening-terms | these terms]]

[Terms of Gardening](gardening-terms.1kfxj)
[Terms of Gardening](1kfxj)

#### These get detected as links and result in not found, but that's expected

Flipping the Wiki link syntax around (putting the label on the left of the `|`
character) does not affect the parsing.

[[these terms | gardening-terms]]
[[these terms | Digital-Garden/gardening-terms.1kfxj]]
[[these terms | Digital-Garden/gardening-terms.1kfxj.md]]
[[these terms|1kfxj]]
[[these terms | 1kfxj]]

### These work as expected

[[Terms of Gardening]]
[[Digital-Garden/gardening-terms.1kfxj]]
[[Digital-Garden/gardening-terms.1kfxj.md]]
[[gardening-terms]]
[[.1kfxj]]
[[1kfxj]]
[[1kfxj.]]

[Terms of Gardening](Digital-Garden/gardening-terms.1kfxj)
