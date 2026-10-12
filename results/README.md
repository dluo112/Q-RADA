# Reported experiment data

See [the complete readable tables](../docs/RESULTS.md) for benchmark settings and reporting notes.

| CSV | Content | Original LaTeX table |
| --- | --- | --- |
| [llava-1.5-7b.csv](llava-1.5-7b.csv) | 192, 128, and 64 visual tokens | [Excerpt](latex/llava-1.5-7b.tex) |
| [llava-next-7b.csv](llava-next-7b.csv) | Nominal budgets of 640 and 320 | [Excerpt](latex/llava-next-7b.tex) |
| [qwen2.5-vl-7b.csv](qwen2.5-vl-7b.csv) | 128, 256, and 512 visual tokens | [Excerpt](latex/qwen2.5-vl-7b.tex) |
| [llava-video-7b.csv](llava-video-7b.csv) | Video-MME and MVBench, 64 frames | [Excerpt](latex/llava-video-7b.tex) |
| [ablation.csv](ablation.csv) | Query relevance and regional allocation | [Excerpt](latex/ablation.tex) |
| [efficiency-pope.csv](efficiency-pope.csv) | Latency, memory, accuracy, and F1 | [Excerpt](latex/efficiency-pope.tex) |
| [extreme-compression.csv](extreme-compression.csv) | 32-token and 16-token evaluation | [Excerpt](latex/extreme-compression.tex) |
| [llava-1.5-13b.csv](llava-1.5-13b.csv) | Transfer to the 13B model | [Excerpt](latex/llava-1.5-13b.tex) |

Data come from `zdy.tex`. [sources.json](sources.json) records table labels, source line numbers, row counts, and the source checksum. The CSV files preserve reported numeric precision. Method names retain the manuscript's venue annotations; `V2Drop` is the plain-text spelling of V²Drop. Percentages retain `%`, and speedup values use `x`.

In `llava-next-7b.csv`, `Full` denotes the unpruned baseline without assigning a fixed token count. The efficiency CSV separately reports average assembled token counts. In the video CSV, token settings are represented as `64 x 169`, `64 x 32`, and `64 x 16`.

The LaTeX excerpts preserve the selected table environments, with line endings and trailing whitespace normalized. They depend on the original manuscript's packages and are supplied as source records, not standalone compilable documents.
