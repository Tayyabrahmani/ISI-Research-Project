# Spatial Analysis of Amino Acid Patterns

This repository contains R code for performing spatial analysis of amino acid patterns in biological sequences. The code utilizes various functions from `stringr`, `mmand`, and `ape` libraries for pattern recognition, frequency analysis, morphological operations, and phylogenetic tree construction. Below, you will find documentation on how to use the code and its functionalities. 
Olfaction plays a crucial role in insects, including the common fruit fly Drosophila melanogaster. Drosophila melanogaster possesses 66 distinct olfactory receptor protein sequences, showcasing significant diversity. This article presents a novel approach for clustering these 66 protein sequences using image-based similarity indices derived from mathematical morphology. Two distinct methodologies are explored: one leveraging the natural occurrence of the twenty standard amino acids, while the other employs chemical grouping of amino acids. A specific metric is devised to facilitate clustering of pairs of sequences based on their similarity indices, categorizing them into three classes: Highest, Moderate, and Least. Notably, OR83b emerges as a prominent olfactory receptor expressed across diverse insect populations, a finding corroborated quantitatively through our investigation.

## Installation

To run the code, you need to have R installed on your system along with the following libraries:

- `stringr`
- `mmand`
- `ape`

You can install these libraries using the following R commands:

```R
install.packages("stringr")
install.packages("mmand")
install.packages("ape")
```

## Usage
1. **Clone the Repository:**
```
git clone https://github.com/tayyabrahmani/Protein-Sequence-analysis.git
```

2. **Prepare Data:**
Ensure that your data is in the appropriate format. For the amino acid analysis, the sequences should be in a file named drosophilaaligned.txt. Each sequence should be separated by a newline character.

3. **Run the R Script:**
Open RStudio or any R environment and run the script algorithm.R. Ensure that all required libraries are loaded.

4. **Interpret Results:**
After running the script, you will get various outputs including heatmaps, dendrograms, and phylogenetic trees. Interpret these results based on your analysis requirements.

## Code Overview
The code performs the following main tasks:

- **Pattern Recognition:** Defines amino acid patterns and identifies their frequencies in biological sequences.
- **Infima and Suprema Calculation:** Computes infima and suprema matrices based on the identified patterns.
- **Area Interaction Matrix:** Calculates area interaction matrices using infima and suprema matrices.
- **Grayscale Morphological Operations:** Performs grayscale morphological dilation and erosion operations to compute distances.
- **Ranking Spatial Fields:** Ranks pairs of spatial fields based on spatial interactions.
- **Phylogenetic Tree Construction:** Constructs phylogenetic trees and dendrograms based on the spatial analysis results.
