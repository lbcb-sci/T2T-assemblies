# Telomere-to-Telomere(T2T) assembly of the human genome

## Data

Oxford Nanopore(ONT), Ultra-long Nanopore sequencing(ULONT) and PacBio HiFi reads were available for the individual with 48x coverage of PacBio Hifi, 70x coverage of ONT and 119x coverage of ULONT reads. Individual's parental ONT and PacBio Hifi reads were also available. The coverage was 28x and 24x for PacBio Hifi and 61x and 67x for ONT reads, respectively, for the paternal and maternal genome sequences. More detailed statistics are given in the tables below. 


### Detailed data statistics
PacBio HiFi

 | SampleID       | Reads          | Total bases    | Min length  | Max length  | Avg length | Coverage |# of SMRT Cells|
 |---------------|----------------|----------------|-------------|-------------|------------|----------|---------------|
 | I002A         | 4.802.282      | 85.073.329.601    | 107 | 50.129  | 17.710,25 | 28,36|2|
 | I002B         | 3.835.379      | 70.674.224.318    | 84  | 57.547  | 18.426,80 | 23,56 |2|
 | I002C         | 8.471.894      | 144.223.668.433    | 45  | 69.921  | 16.854,02 | 48,07 |3+2|

ONT                                                      
 
 | SampleID       | Reads          | Total bases    | Min length  | Max length  | Avg length | Coverage |
 |---------------|----------------|----------------|-------------|-------------|------------|----------|
 | I002A         | 10.461.323      | 185.316.102.673    | 1 | 392.252  | 17.715,00 | 61,77|
 | I002B         | 13.605.232      | 202.049.459.153    | 1  | 297.466  | 14.851,61 | 67,35 |
 | I002C         | 22.540.612      | 208.364.758.587    | 1  | 415.645  | 9.273,40 | 69,45 |
 
 
ULONT                                                     
 
 | SampleID       | Reads          | Total bases    | Min length  | Max length  | Avg length | Coverage |
 |---------------|----------------|----------------|-------------|-------------|------------|----------|
 | I002A         | -      | -   | - | -  | - | - |
 | I002B         | -      | -   | - | -  | - | - |
 | I002C         | 10.734.062      | 460.099.466.537    | 9  | 1.543.464  | 42.863,50 | 119,34 |
 
 
# Assembly  releases 

## Reference

For assembly evaluation, the [T2T-CHM13v2.0](https://www.ncbi.nlm.nih.gov/assembly/GCA_009914755.4) reference was used.

## v0.1

The assembly was created using [hifiasm](https://github.com/chhylp123/hifiasm) utilizing trio-binning to produce a phased diploid assembly.

Haplotype 1 is available at [link](https://humangenomereferencelbcb1.s3.eu-central-1.amazonaws.com/hifiasm.trio.ulont.100k.nochimmerlig.asm.bp.hap1.p_ctg.fa) 

Haplotype 2 is available at [link](https://humangenomereferencelbcb1.s3.eu-central-1.amazonaws.com/hifiasm.trio.ulont.100k.nochimmerlig.asm.bp.hap2.p_ctg.fa)

Hifi reads were beforehand procured using [DeepConsensus](https://github.com/google/deepconsensus).

[Merlion](https://github.com/lbcb-sci/merlion) and [Liger2LiGer](https://github.com/rlorigro/Liger2LiGer) were used to detect UL ONT chimeric reads.

 
 
| | Haplotype 1 | Haplotype 2 |
|--------|---------|--------|
| NGA50 | 80.078.556 | 57.165.402 |
| N50 | 90.737.878 | 73.421.881 |
| # contigs | 335 | 277 |

### D-Genies plots - assemblies vs reference
![](https://github.com/lbcb-sci/T2T-assemblies/blob/main/data/v0.1-human-assembly-to-reference.png)
