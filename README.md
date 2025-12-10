# GEO_HaT_Xenium_Submission

Analysis of spatial transcriptomic differences between HaT and non-HaT colon samples using Xenium spatial transcriptomics.

## Repository Structure

```
├── raw_data/           # Unaltered Xenium exports from 10x Genomics
├── processed_data/     # Aggregated counts, DESeq2 results, normalized matrices
├── code/               # R Markdown and scripts for analysis and figure generation
└── figures/            # Manuscript figures
```

## Requirements

- R ≥ 4.3
- Seurat v5
- DESeq2
- ggplot2
- ggrepel

## Installation

```r
# Install required packages
install.packages(c("Seurat", "ggplot2", "ggrepel"))
BiocManager::install("DESeq2")
```

## Usage

Detailed analysis scripts are provided in the `code/` directory. Start with the main analysis pipeline to reproduce figures and results.

## Citation

If you use this data or code, please cite our publication (citation will be added upon acceptance).

## Contact

**Glover Lab**  
Tulane University  
📧 gloverlab@tulane.edu

## License

[Add appropriate license]
