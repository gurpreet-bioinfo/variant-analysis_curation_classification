### ❓ What are Genomic Variants from omics (WGS/WES) data and what scientific concepts should you know for stress-free, organized and accurate variant curation and classification? 🎯 

### 💡 Concepts to know:

###  Genomic Variants Definition: 
Differences in DNA sequences among human genomes, detected either in coding regions (via WES) or across the entire genome (via WGS) and central to understanding health-related traits and diseases | https://www.genome.gov/about-genomics/educational-resources/fact-sheets/human-genomic-variation 

### Variant  Curation and Classification:
#### (I) Based on various criteria and the American College of Medical Genetics and Genomics and the Association for Molecular Pathology (ACMG-AMP) system:
1. Minor Allele Frequency (MAF) as per Genome Aggregation Database (gnomAD) | https://pubmed.ncbi.nlm.nih.gov/34889978/ , https://pubmed.ncbi.nlm.nih.gov/34859531/ , https://pubmed.ncbi.nlm.nih.gov/35856030
    - MAF < 0.000001 %     =>  Hyper-rare
    - 0.001% < MAF < 0.1%  =>  Ultra-rare
    - 0.1% ≤ MAF < 1%      =>  Rare
    - 1% ≤ MAF < 5%        =>  Low-frequency
    - MAF ≥ 5%             =>  Common 

2. Computational predictive tools | https://pubmed.ncbi.nlm.nih.gov/25741868/
    - Missense prediction
    - Splice site prediction
    - Nucleotide conservation prediction

3. Clinical Significance | https://pubmed.ncbi.nlm.nih.gov/25741868
    - Pathogenic (P)
    - Likely Pathogenic (LP)
    - Variant of Uncertain Significance (VUS)
    - Likely Benign (LB)
    - Benign (B)

4. Evidence Framework | https://pubmed.ncbi.nlm.nih.gov/25741868/ 
    - Criteria of pathogenicity
        - Very strong: PVS1
        - Strong: PS1, PS2, PS3, PS4
        - Moderate: PM1, PM2, PM3, PM4, PM5, PM6
        - Supporting: PP1, PP2, PP3, PP4, PP5
    - Benign
        - Stand-alone: BA1
        - Strong: BS1, BS2, BS3, BS4
        - Supporting: BP1, BP2, BP3, BP4, BP5, BP6, BP7

5. Disease-associated variant class | https://pubmed.ncbi.nlm.nih.gov/37982373/ , https://pubmed.ncbi.nlm.nih.gov/37234922/ Fig 4
    - Non-synonymous (Missense)
    - Synonymous
    - Splicing
    - UTR
    - Intronic
    - Regulatory

6. Disease-associated variant consequence | https://pubmed.ncbi.nlm.nih.gov/37982373/
    - Altered gene product level
    - Increased gene product level
    - Decreased gene product level
    - Absent gene product
    - Altered gene product sequence
    - Functionally normal

7. HPO (Human Phenotype Ontology) Mode of Inheritance | https://pubmed.ncbi.nlm.nih.gov/37982373/
    - Allelic Requirement | Mendelian Inheritance Term
        - monoallelic_autosomal  | Autosomal Dominant (AD)  
        - biallelic_autosomal | Autosomal Recessive (AR) 
        - monoallelic_X_heterozygous | X-linked Dominant
        - monoallelic_X_hemizygous | X-linked Recessive
        - monoallelic_Y_hemizygous | Y-Linked 
        - mitochondrial | Mitochondrial
        - monoallelic_PAR | PAR dominant
        - biallelic_PAR | PAR recessive
    - Non-Mendelian Inheritance
        - Digenic
        - Multigenic/Complex
    - Additional Context / Optional Terms
        - De novo (new)
        - Somatic mosaicism
        - Incomplete penetrance
        - Complete penetrance
        - Highly variable age of onset
        - Age-related onset
        - Imprinted: maternal or paternal
        - Repeat expansion
        - Requires heterozygosity
        - Sex-limited expression
        - Contiguous gene syndrome

8. Type of alteration | https://www.genome.gov/about-genomics/educational-resources/fact-sheets/human-genomic-variation
    - Single Nucleotide Variant (SNV)
    - Insertion (INS)
    - Deletion (DEL)
    - Copy Number Variant (CNV)

9. Cell type (origin) | https://pubmed.ncbi.nlm.nih.gov/32498674/ 
    - Germline (heritable)
    - Somatic
    - Shared

#### (II) Based on ABC system | https://pubmed.ncbi.nlm.nih.gov/33981013/ , https://pubmed.ncbi.nlm.nih.gov/38778080/ 

1. Step A: Functional grading (functional classes)
    - functional VUS (fVUS)
    - Normal function (NF)
    - Likely normal function (LNF)
    - Hypothetical functional effect (HFE)
    - Likely functional effect (LFE)
    - Functional effect (FE)

2. Step B: Clinical grading (clinical classes)
    - clinical VUS (cVUS)
    - Variant of potential interest (VOI)
    - Known or assumed risk factor variant
    - Pathogenic variant
    - Moderate penetrance pathogenic variant
    - High penetrance pathogenic variant

3. Combined A+B class
    - 0: Not reported
    - F: Not reported; gene is unrelated to the phenotype
    - E: Variant of potential interest (VOI) 
    - D: Low penetrance and good candidate
    - C: Pathogenic: disease-associated variant
    - B: Pathogenic: disease-associated variant of moderate penetrance 
    - A: Pathogenic: disease-associated variant of high penetrance
    - X: Secondary/incidental finding

4. Step C: Selection of standard variant comment based on combined class C
    - 0: Normal findings 
    - F: Normal findings - No P/LP 
    - F/E: Normal findings - No P variants related to the phenotype
    - E/D: Normal findings - No P variants to explain the phenotype
    - E/D: Genetic variant of potential interest
    - E/D: Heterozygosity for a recessive genetic variant of potential interest
    - D: Genetic variant that increases susceptibility for this phenotype
    - C/B/A: Disease-associated pathogenic variant
    - X: Genetic variant unrelated to the clinical question

### Tutorial
Refer 📌 tutorial here: https://github.com/gurpreet-bioinfo/vcf_concepts_analysis_visualization/tree/main to explore and interactively visualize a VCF file using free web-based tools, and hands-on with the above **concepts**.
