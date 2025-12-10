# GEO_HaT_Xenium_Submission

## Overview

This repository supports our investigation into mast cell phenotypes in Hereditary α-tryptasemia (HαT) and inflammatory bowel disease (IBD). Using spatial transcriptomics, we demonstrate that HαT is associated with increased gastrointestinal mast cell abundance and elevated expression of MRGPRX2, a non-IgE activation receptor that may contribute to gastrointestinal symptoms in these patients.

## Background

Hereditary α-tryptasemia (HαT) is characterized by increased *TPSAB1* copy number and elevated basal serum tryptase. While associated with mast cell-mediated symptoms, its role in gastrointestinal disease has remained unclear. This study examined MRGPRX2 expression patterns in individuals with HαT and IBD using multiple complementary approaches:

- **Genotyping**: 854 biobanked IBD samples
- **Spatial transcriptomics**: Descending colon tissue (4 HαT, 4 non-HαT)
- **Mass cytometry (CyTOF)**: Small-intestinal biopsies (5 HαT, 12 controls)

## Key Findings

Our multi-platform analysis revealed that HαT is associated with:
- Increased gastrointestinal mast cell abundance
- Elevated expression of activation markers (CD203c, LAMP-1, SIGLEC8)
- Significantly increased *MRGPRX2* and *SIGLEC8* transcripts in IBD samples from HαT individuals

These findings suggest enhanced MRGPRX2 expression and mast cell activation may contribute to gastrointestinal symptoms in HαT, particularly in IBD contexts. As precision immunogenetics advances, defining mast cell phenotypes linked to α-tryptase copy number may refine diagnostic approaches and identify candidates for emerging mast cell-targeted therapies.

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

MIT License

Copyright (c) 2024 Glover Lab, Tulane University

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
