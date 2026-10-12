# Figure assets and provenance

[Project overview](../README.md)

Figures are copied from the Q-RADA manuscript assets and rendered to PNG at a maximum dimension of 2,400 pixels for GitHub display. The vector PDFs preserve the original files without modification.

| Figure | PNG preview | Original vector PDF | Source asset |
| --- | --- | --- | --- |
| Method overview | [PNG](../assets/figures/overview.png) | [PDF](../assets/pdf/overview.pdf) | `Figure/overview.pdf` |
| Motivation | [PNG](../assets/figures/motivation.png) | [PDF](../assets/pdf/motivation.pdf) | `Figure/introduction1.pdf` |
| Regional distortion and surrogate gains | [PNG](../assets/figures/regional-curves.png) | [PDF](../assets/pdf/regional-curves.pdf) | `Figure/regional_curves.pdf` |
| Parameter sensitivity | [PNG](../assets/figures/parameter-sensitivity.png) | [PDF](../assets/pdf/parameter-sensitivity.pdf) | `Figure/h_k_surface_corrected_cropped.pdf` |
| Query-aware token allocation | [PNG](../assets/figures/token-visualization.png) | [PDF](../assets/pdf/token-visualization.pdf) | `Figure/CDPruner_all_cases_single_slide_cropped.pdf` |

The token-allocation asset's original filename contains `CDPruner`; its role here is the Q-RADA visualization identified by `fig:token-visualization` and its caption in `zdy.tex`. Its compressed columns are labeled `B=64` and `B=128`.

The overview is a schematic illustration. The exact surrogate-gain definition and allocation rule are explained in the README and manuscript. `B` denotes the global token budget, `K` the eligible-region cap, and `k` a regional rate in the method text; some schematic axes use `K` for token count.

[Source manifest](../results/sources.json) records original asset names, SHA-256 checksums, and the manuscript source used for table extraction. The LaTeX manuscript and reviewer response files are retained in the author workspace and are not part of this repository.
