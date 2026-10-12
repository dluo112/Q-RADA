# Experimental results

[Project overview](../README.md) · [Download CSV tables](../results/)

These are results reported in the Q-RADA manuscript, transcribed from `zdy.tex`. They have not been rerun in this repository; implementation and evaluation code are pending release. Each table includes its original LaTeX excerpt for checking the transcription.

`Avg.%` is the manuscript-reported relative aggregate score, with each table's full-token reference set to 100%. It is not an arithmetic mean of raw benchmark scores. The manuscript does not specify an explicit aggregate formula, so the reported values are preserved without recalculation. Values above 100% refer to the aggregate, rather than improvements on every benchmark. Benchmark scores retain their original scales, including MME.

## LLaVA-1.5-7B

The full-token reference uses 576 visual tokens. Avg.% is the manuscript-reported relative aggregate score over eight benchmarks.

Source label: `tab:results-7b`. [CSV](../results/llava-1.5-7b.csv) · [LaTeX](../results/latex/llava-1.5-7b.tex)

### Retained tokens: 192

| Method | Tokens | SEED (Img) | MME | TextVQA | MMB (EN) | VizWiz | SQA | GQA | POPE | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| LLaVA-1.5-7B | 576 | 66.2 | 1862.0 | 58.2 | 64.7 | 50.1 | 69.5 | 61.9 | 85.9 | 100.0% |
| FastV (ECCV'24) | 192 | 63.6 | 1612.0 | 52.5 | 61.2 | 50.8 | 67.3 | 52.7 | 64.8 | 89.8% |
| SparseVLM (ICML'25) | 192 | 64.2 | 1721.0 | 56.1 | 62.5 | 50.5 | 69.1 | 57.6 | 83.6 | 96.4% |
| VisionZip (CVPR'25) | 192 | 64.7 | 1783.0 | 57.3 | 63.0 | 52.3 | 68.9 | 59.3 | 85.3 | 98.2% |
| SCOPE (NeurIPS'25) | 192 | 64.4 | 1804.0 | 57.7 | 63.6 | 52.4 | 68.8 | 60.1 | 86.4 | 98.9% |
| V2Drop (CVPR'26) | 192 | 63.5 | 1826.0 | 55.6 | 63.7 | 53.6 | 69.3 | 58.5 | 85.1 | 98.4% |
| Q-RADA (ours) | 192 | 65.0 | 1819.0 | 56.6 | 63.8 | 54.3 | 69.5 | 60.2 | 87.6 | 99.7% |

### Retained tokens: 128

| Method | Tokens | SEED (Img) | MME | TextVQA | MMB (EN) | VizWiz | SQA | GQA | POPE | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| LLaVA-1.5-7B | 576 | 66.2 | 1862.0 | 58.2 | 64.7 | 50.1 | 69.5 | 61.9 | 85.9 | 100.0% |
| FastV (ECCV'24) | 128 | 61.4 | 1490.0 | 50.6 | 56.1 | 51.9 | 60.2 | 49.6 | 59.6 | 84.4% |
| SparseVLM (ICML'25) | 128 | 63.6 | 1696.0 | 54.9 | 60.0 | 49.4 | 67.1 | 56.0 | 80.5 | 93.9% |
| VisionZip (CVPR'25) | 128 | 63.8 | 1762.0 | 56.8 | 62.0 | 51.6 | 68.9 | 57.6 | 83.2 | 96.8% |
| DART (EMNLP'25) | 128 | 63.4 | 1721.0 | 56.3 | 60.7 | 52.8 | 69.1 | 57.9 | 80.4 | 95.8% |
| DivPrune (CVPR'25) | 128 | 62.3 | 1718.0 | 56.1 | 62.0 | 52.8 | 69.0 | 59.3 | 86.7 | 97.2% |
| SCOPE (NeurIPS'25) | 128 | 63.6 | 1776.0 | 57.2 | 62.5 | 52.3 | 68.4 | 59.7 | 86.1 | 98.0% |
| V2Drop (CVPR'26) | 128 | 62.7 | 1712.0 | 53.8 | 61.8 | 53.7 | 68.8 | 56.3 | 80.9 | 95.3% |
| AgilePruner (ICLR'26) | 128 | 64.2 | 1748.0 | 57.0 | 61.8 | 53.0 | 68.6 | 59.4 | 87.4 | 98.0% |
| Q-RADA (ours) | 128 | 64.3 | 1769.0 | 56.1 | 63.4 | 54.2 | 69.2 | 59.3 | 87.2 | 98.6% |

### Retained tokens: 64

| Method | Tokens | SEED (Img) | MME | TextVQA | MMB (EN) | VizWiz | SQA | GQA | POPE | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| LLaVA-1.5-7B | 576 | 66.2 | 1862.0 | 58.2 | 64.7 | 50.1 | 69.5 | 61.9 | 85.9 | 100.0% |
| FastV (ECCV'24) | 64 | 55.4 | 1256.0 | 47.8 | 48.0 | 49.1 | 51.1 | 46.1 | 48.0 | 74.3% |
| SparseVLM (ICML'25) | 64 | 56.7 | 1505.0 | 51.8 | 56.2 | 49.4 | 62.2 | 52.7 | 75.1 | 87.2% |
| VisionZip (CVPR'25) | 64 | 60.5 | 1690.0 | 55.5 | 60.1 | 52.9 | 69.0 | 55.1 | 77.0 | 93.6% |
| DART (EMNLP'25) | 64 | 59.2 | 1705.0 | 54.7 | 59.5 | 53.5 | 69.3 | 54.7 | 73.9 | 92.8% |
| DivPrune (CVPR'25) | 64 | 60.1 | 1674.0 | 54.7 | 59.3 | 53.6 | 68.2 | 57.8 | 85.6 | 95.2% |
| SCOPE (NeurIPS'25) | 64 | 61.6 | 1698.0 | 56.6 | 61.7 | 53.6 | 68.6 | 58.3 | 86.4 | 96.7% |
| V2Drop (CVPR'26) | 64 | 59.7 | 1470.0 | 51.8 | 55.2 | 50.1 | 68.9 | 50.5 | 75.1 | 88.2% |
| AgilePruner (ICLR'26) | 64 | 62.3 | 1703.0 | 56.0 | 60.7 | 54.0 | 68.6 | 57.4 | 74.1 | 94.3% |
| Q-RADA (ours) | 64 | 62.6 | 1727.0 | 53.5 | 61.6 | 55.0 | 68.5 | 58.5 | 87.5 | 97.1% |


## LLaVA-NeXT-7B

The budgets in this accuracy table are nominal retained projected-token budgets. They differ from the average assembled visual-token counts reported in the efficiency table. Acc. and Avg.% follow the manuscript reporting.

Source label: `tab:results-next-7b`. [CSV](../results/llava-next-7b.csv) · [LaTeX](../results/latex/llava-next-7b.tex)

### Retained tokens: 640

| Method | Tokens | SEED (Img) | MME | MMB (EN) | VizWiz | SQA | GQA | POPE | Acc. | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| LLaVA-NeXT-7B | Full | 70.2 | 1512 | 65.8 | 55.2 | 67.5 | 62.5 | 86.8 | 69.1 | 100.0% |
| FastV (ECCV'24) | 640 | 63.7 | 1412 | 63.1 | 53.9 | 67.4 | 58.9 | 79.5 | 65.3 | 94.5% |
| PDrop (CVPR'25) | 640 | 65.5 | 1475 | 64.1 | 53.8 | 66.7 | 60.0 | 83.8 | 66.8 | 96.7% |
| SparseVLM (ICML'25) | 640 | 66.2 | 1456 | 65.9 | 53.6 | 67.6 | 61.2 | 85.3 | 67.5 | 97.7% |
| PruMerge+ (ICCV'25) | 640 | 66.8 | 1480 | 64.6 | 57.9 | 67.8 | 60.8 | 85.3 | 68.2 | 98.7% |
| VisionZip (CVPR'25) | 640 | 67.1 | 1493 | 65.8 | 57.1 | 68.1 | 61.2 | 86.0 | 68.6 | 99.2% |
| DivPrune (CVPR'25) | 640 | 67.5 | 1469 | 65.8 | 55.7 | 67.8 | 61.9 | 86.9 | 68.4 | 99.0% |
| AgilePruner (ICLR'26) | 640 | 67.3 | 1502 | 65.9 | 56 | 67.8 | 62 | 86.1 | 68.6 | 99.3% |
| Q-RADA (ours) | 640 | 68.6 | 1480 | 66.1 | 58.02 | 68.22 | 63.55 | 88.34 | 69.5 | 100.6% |

### Retained tokens: 320

| Method | Tokens | SEED (Img) | MME | MMB (EN) | VizWiz | SQA | GQA | POPE | Acc. | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| LLaVA-NeXT-7B | Full | 70.2 | 1512 | 65.8 | 55.2 | 67.5 | 62.5 | 86.8 | 69.1 | 100.0% |
| FastV (ECCV'24) | 320 | 62.6 | 1099 | 53.4 | 51.3 | 66.6 | 49.8 | 49.5 | 55.5 | 80.2% |
| PDrop (CVPR'25) | 320 | 64.6 | 1171 | 55.5 | 49.7 | 66.7 | 50.4 | 60.8 | 58.0 | 84.0% |
| SparseVLM (ICML'25) | 320 | 65.1 | 1386 | 63.1 | 54.2 | 67.2 | 57.9 | 76.9 | 64.8 | 93.8% |
| PruMerge+ (ICCV'25) | 320 | 64.4 | 1444 | 63 | 57.7 | 68.1 | 58.8 | 79.5 | 66.2 | 95.9% |
| VisionZip (CVPR'25) | 320 | 65.3 | 1397 | 63.3 | 56.2 | 67.5 | 58.9 | 82.3 | 66.2 | 95.8% |
| DivPrune (CVPR'25) | 320 | 65.8 | 1423 | 63.9 | 55.6 | 67.7 | 61.1 | 84.7 | 67.1 | 97.2% |
| AgilePruner (ICLR'26) | 320 | 65.7 | 1475 | 64.5 | 55.8 | 67.3 | 60.1 | 84 | 67.3 | 97.4% |
| Q-RADA (ours) | 320 | 66.2 | 1451 | 64 | 55.83 | 67.58 | 61.74 | 88.24 | 68.0 | 98.4% |


## Qwen2.5-VL-7B

The full-token reference uses 1,296 visual tokens. Acc. and Avg.% follow the manuscript reporting over eight benchmarks.

Source label: `tab:token_budget_comparison`. [CSV](../results/qwen2.5-vl-7b.csv) · [LaTeX](../results/latex/qwen2.5-vl-7b.tex)

### Retained tokens: 128

| Method | Tokens | AI2D | MME | MMStar | MMB-EN | POPE | MMB-CN | SQA-IMG | RealWorldQA | Acc. | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Qwen2.5-VL-7B | 1296 | 80.3 | 2322.0 | 63.9 | 82.8 | 87.7 | 83.2 | 88.2 | 66.3 | 83.6 | 100.0% |
| FastV (ECCV'24) | 128 | 71.4 | 1979.0 | 37.4 | 72.9 | 75.8 | 72.2 | 69.4 | 57.8 | 69.5 | 83.1% |
| DivPrune (CVPR'25) | 128 | 72.1 | 2028.0 | 45.1 | 77.8 | 81.8 | 77.8 | 68.6 | 57.9 | 72.8 | 87.1% |
| CDPruner (NeurIPS'25) | 128 | 74.0 | 2127.0 | 51.7 | 76.2 | 75.6 | 76.5 | 69.3 | 59.1 | 73.6 | 88.1% |
| HAWK (CVPR'26) | 128 | 75.0 | 2137.0 | 51.5 | 75.8 | 77.8 | 75.7 | 70.2 | 59.4 | 74.0 | 88.6% |
| Q-RADA (ours) | 128 | 75.7 | 2234.0 | 53.3 | 79.8 | 88.9 | 76.4 | 86.4 | 64.1 | 79.5 | 95.2% |

### Retained tokens: 256

| Method | Tokens | AI2D | MME | MMStar | MMB-EN | POPE | MMB-CN | SQA-IMG | RealWorldQA | Acc. | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Qwen2.5-VL-7B | 1296 | 80.3 | 2322.0 | 63.9 | 82.8 | 87.7 | 83.2 | 88.2 | 66.3 | 83.6 | 100.0% |
| FastV (ECCV'24) | 256 | 76.2 | 2233.0 | 41.8 | 79.6 | 81.2 | 78.9 | 70.9 | 62.5 | 75.3 | 90.2% |
| DivPrune (CVPR'25) | 256 | 76.5 | 2162.0 | 48.3 | 80.0 | 83.5 | 79.6 | 70.1 | 60.5 | 75.8 | 90.7% |
| CDPruner (NeurIPS'25) | 256 | 77.5 | 2245.0 | 57.4 | 80.9 | 79.4 | 79.9 | 70.7 | 62.2 | 77.5 | 92.8% |
| HAWK (CVPR'26) | 256 | 77.7 | 2245.0 | 57.9 | 81.1 | 82.9 | 79.4 | 71.9 | 63.7 | 78.4 | 93.8% |
| Q-RADA (ours) | 256 | 80.4 | 2316.0 | 58.3 | 82.0 | 88.6 | 80.1 | 88.1 | 64.2 | 82.2 | 98.4% |

### Retained tokens: 512

| Method | Tokens | AI2D | MME | MMStar | MMB-EN | POPE | MMB-CN | SQA-IMG | RealWorldQA | Acc. | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| Qwen2.5-VL-7B | 1296 | 80.3 | 2322.0 | 63.9 | 82.8 | 87.7 | 83.2 | 88.2 | 66.3 | 83.6 | 100.0% |
| FastV (ECCV'24) | 512 | 78.8 | 2318.0 | 58.5 | 82.0 | 84.0 | 81.8 | 71.5 | 64.7 | 79.7 | 95.3% |
| DivPrune (CVPR'25) | 512 | 78.6 | 2258.0 | 61.9 | 81.6 | 84.4 | 82.1 | 71.0 | 63.8 | 79.5 | 95.2% |
| CDPruner (NeurIPS'25) | 512 | 78.9 | 2327.0 | 63.1 | 82.2 | 82.6 | 82.6 | 71.3 | 64.8 | 80.2 | 96.0% |
| HAWK (CVPR'26) | 512 | 79.6 | 2342.0 | 63.3 | 82.5 | 85.0 | 82.3 | 72.6 | 65.4 | 81.0 | 96.9% |
| Q-RADA (ours) | 512 | 83.4 | 2340.0 | 63.4 | 83.8 | 88.1 | 82.9 | 88.5 | 64.8 | 84.0 | 100.5% |


## LLaVA-Video-7B

The experiment uses 64 frames. Token budgets are written as frames x retained tokens per frame; the full-token reference is 64 x 169.

Source label: `tab:experiment`. [CSV](../results/llava-video-7b.csv) · [LaTeX](../results/latex/llava-video-7b.tex)

### Retained tokens: 64 x 32

| Method | Frames x tokens/frame | Video-MME Short | Video-MME Medium | Video-MME Long | MVBench |
| --- | --- | --- | --- | --- | --- |
| LLaVA-Video-7B | 64 x 169 | 76.6 | 61.2 | 53.1 | 58.2 |
| FastV (ECCV'24) | 64 x 32 | 63.8 | 55.9 | 48.4 | 52.7 |
| PDrop (CVPR'25) | 64 x 32 | 67.0 | 57.7 | 50.0 | 53.1 |
| SparseVLM (ICML'25) | 64 x 32 | 69.8 | 56.9 | 50.3 | 54.1 |
| DART (EMNLP'25) | 64 x 32 | 67.3 | 57.1 | 50.0 | 52.7 |
| DivPrune (CVPR'25) | 64 x 32 | 69.9 | 57.9 | 50.2 | 53.7 |
| CDPruner (NeurIPS'25) | 64 x 32 | 71.9 | 58.6 | 51.0 | 55.7 |
| Q-RADA (ours) | 64 x 32 | 71.9 | 58.9 | 51.1 | 60.3 |

### Retained tokens: 64 x 16

| Method | Frames x tokens/frame | Video-MME Short | Video-MME Medium | Video-MME Long | MVBench |
| --- | --- | --- | --- | --- | --- |
| LLaVA-Video-7B | 64 x 169 | 76.6 | 61.2 | 53.1 | 58.2 |
| FastV (ECCV'24) | 64 x 16 | 55.0 | 50.0 | 45.0 | 46.8 |
| PDrop (CVPR'25) | 64 x 16 | 52.9 | 50.0 | 43.8 | 44.3 |
| SparseVLM (ICML'25) | 64 x 16 | 53.8 | 49.3 | 46.3 | 48.7 |
| DART (EMNLP'25) | 64 x 16 | 64.8 | 52.9 | 48.1 | 50.4 |
| DivPrune (CVPR'25) | 64 x 16 | 67.7 | 54.2 | 48.2 | 52.0 |
| CDPruner (NeurIPS'25) | 64 x 16 | 66.2 | 56.0 | 49.6 | 53.8 |
| Q-RADA (ours) | 64 x 16 | 68.8 | 56.6 | 49.7 | 58.4 |


## Ablation: LLaVA-1.5-7B

Compressed variants use 64 visual tokens. Avg.% covers five benchmarks here; it is a different aggregate from the eight-benchmark 97.1% result in the main LLaVA-1.5-7B table.

Source label: `tab:ablation`. [CSV](../results/ablation.csv) · [LaTeX](../results/latex/ablation.tex)

| Method | Tokens | GQA | MMB | MME | POPE | VizWiz | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- |
| LLaVA-1.5-7B | 576 | 61.9 | 64.7 | 1862 | 85.9 | 50.1 | 100.0% |
| w/o query relevance | 64 | 55.5 | 58.8 | 1630 | 81.5 | 53.1 | 92.9% |
| w/o regional R-D allocation | 64 | 54.7 | 58.1 | 1570 | 83.5 | 53.5 | 92.3% |
| Q-RADA (ours) | 64 | 58.5 | 61.6 | 1727 | 87.5 | 55.0 | 98.1% |

## Efficiency: LLaVA-NeXT-7B on POPE

Counts are average assembled visual tokens across POPE examples. Mean and P95 latency are in seconds; peak memory is in GiB. Speedups were calculated from unrounded mean latencies and are copied as reported, rather than recomputed from the rounded display values. The manuscript reports experiments on two NVIDIA RTX 4090 D GPUs.

Source label: `tab:budget-efficiency`. [CSV](../results/efficiency-pope.csv) · [LaTeX](../results/latex/efficiency-pope.tex)

| Method | Avg. visual tokens | Mean latency (s) | P95 latency (s) | Speedup | Peak memory (GiB) | Accuracy (%) | F1 (%) |
| --- | --- | --- | --- | --- | --- | --- | --- |
| LLaVA-NeXT-7B | 2280 | 0.33 | 0.40 | 1.00x | 15.03 | 86.80 | 86.40 |
| Q-RADA | 320 | 0.21 | 0.23 | 1.57x | 14.65 | 88.24 | 87.02 |
| Q-RADA | 175 | 0.17 | 0.18 | 1.87x | 14.09 | 87.50 | 86.90 |
| Q-RADA | 80 | 0.15 | 0.17 | 2.20x | 13.89 | 86.93 | 86.31 |

## Extreme compression: LLaVA-1.5-7B

Budgets of 32 and 16 tokens reduce the original 576-token sequence by 94.4% and 97.2%, respectively.

Source label: `tab:extreme-compression`. [CSV](../results/extreme-compression.csv) · [LaTeX](../results/latex/extreme-compression.tex)

| Method | Tokens | GQA | MMB | MME | POPE | VizWiz |
| --- | --- | --- | --- | --- | --- | --- |
| LLaVA-1.5-7B | 576 | 61.9 | 64.7 | 1862 | 85.9 | 50.1 |
| VisionZip | 32 | 51.8 | 55.6 | 1545 | 69.8 | 50.5 |
| SCOPE | 32 | 55.7 | 59.4 | 1628 | 80.1 | 52.7 |
| Q-RADA | 32 | 57.9 | 60.8 | 1664 | 84.2 | 53.8 |
| VisionZip | 16 | 43.2 | 45.8 | 1210 | 52.1 | 46.0 |
| SCOPE | 16 | 48.9 | 52.1 | 1398 | 70.4 | 48.1 |
| Q-RADA | 16 | 52.7 | 55.8 | 1492 | 78.6 | 50.9 |

## Transfer: LLaVA-1.5-13B

The full-token 13B reference uses 576 visual tokens. Avg.% covers the five benchmarks in this table.

Source label: `tab:larger-model`. [CSV](../results/llava-1.5-13b.csv) · [LaTeX](../results/latex/llava-1.5-13b.tex)

| Method | Tokens | GQA | MMB | MME | POPE | VizWiz | Avg.% |
| --- | --- | --- | --- | --- | --- | --- | --- |
| LLaVA-1.5-13B | 576 | 63.2 | 67.7 | 1818 | 85.9 | 53.6 | 100.0 |
| SCOPE | 128 | 59.3 | 67.2 | 1735 | 85.9 | 52.2 | 97.3 |
| Q-RADA | 128 | 60.4 | 66.3 | 1752 | 87.5 | 53.6 | 98.4 |
| SCOPE | 64 | 58.7 | 65.5 | 1762 | 83.0 | 51.5 | 96.0 |
| Q-RADA | 64 | 60.1 | 64.6 | 1715 | 87.1 | 53.8 | 97.2 |
