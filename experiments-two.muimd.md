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
[[these terms|1kfxj]]
[[these terms | 1kfxj]]
[[.1kfxj | these terms]]
[[1kfxj. | foo]]
[[these terms | Digital-Garden/gardening-terms.1kfxj]]
[[Digital-Garden/gardening-terms.1kfxj | these terms]]
[[these terms | gardening-terms]]
[[Digital-Garden/gardening-terms.1kfxj.md | these terms]]
[[these terms | Digital-Garden/gardening-terms.1kfxj.md]]
[[gardening-terms | these terms]]

[Terms of Gardening](gardening-terms.1kfxj)
[Terms of Gardening](1kfxj)

### These work as expected

[[Terms of Gardening]]
[[Digital-Garden/gardening-terms.1kfxj]]
[[Digital-Garden/gardening-terms.1kfxj.md]]
[[gardening-terms]]
[[.1kfxj]]
[[1kfxj]]
[[1kfxj.]]

[Terms of Gardening](Digital-Garden/gardening-terms.1kfxj)
