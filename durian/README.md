# Telomere-to-Telomere(T2T) assembly of the durian genome


## Data


### Data coverage statistics
||Coverage|
|-|-|
|PacBio Hifi|~60x|
|UL ONT(>100kbp)|~30x|
|OMNI-C|~60x|

 
 
# Assembly  releases 
## Reference
For assembly evaluation, the current Durian [reference](https://www.nature.com/articles/ng.3972) was used.


## v0.1

The assembly was created using [hifiasm](https://github.com/chhylp123/hifiasm) utilizing Hi-C reads to produce a phased diploid assembly.

Haplotype 1 is available at [link](https://drive.google.com/file/d/1yPfw6y17zuia1zhvDXG95gpF4MTZHe5g/view?usp=sharing)

Haplotype 2 is available at [link](https://drive.google.com/file/d/1t3hSNTiggkVMKiILsE8PShcATYy3WkU4/view?usp=sharing)
 
 
| | Haplotype 1 | Haplotype 2 |
|--------|---------|--------|
| NG50 | 20.685.927 | 21.459.630 |
| # contigs | 599 | 353 |
| # contigs >= 3Mbp | 45 | 45 |
| # contigs* with TR** at both endings | 12 | 11 |
| # contigs* with TR** at one of the endings | 28 | 28 |
| # contigs* with no TR** at the endings | 5 | 6 |

contigs* - contigs larger or equal to 3Mbp

TR** - tandem repeats specific for telomeres (ACCCTAA/TTAGGGT)


 
## v0.2

The assembly was created using [hifiasm](https://github.com/chhylp123/hifiasm) utilizing Hi-C reads to produce a phased diploid assembly.

Haplotype 1 is available at [link](https://drive.google.com/file/d/1w1BmmBogn6NnHxCoJfX60yoYJY-rjmRo/view?usp=sharing)

Haplotype 2 is available at [link](https://drive.google.com/file/d/1LuvwGmWjC7bhXs973QUum8Y0ydohl_gT/view?usp=sharing)

Hifi reads were beforehand procured using [DeepConsensus](https://github.com/google/deepconsensus).

[Merlion](https://github.com/lbcb-sci/merlion) was used to detect UL ONT chimeric reads.


|Reads longer than 100kbp| Chimeric reads | % of chimeric reads |
|------------------------|----------------|---------------------|
|139.949|49.346|35,26|
 
 
| | Haplotype 1 | Haplotype 2 |
|--------|---------|--------|     
| NG50 | 21.458.057 | 22.634.734 |
| # contigs | 370 | 299 |
| # contigs >= 3Mbp | 43 | 40 |
| # contigs* with TR** at both endings | 13 | 14 |
| # contigs* with TR** at one of the endings | 25 | 22 |
| # contigs* with no TR** at the endings | 5 | 4 |

contigs* - contigs larger or equal to 3Mbp

TR** - tandem repeats specific for telomeres (ACCCTAA/TTAGGGT)



## v0.3

The results of the first rounds of manual scaffolding using assembly v0.2. 

For manual scaffolding HiC reads were mapped to assembly using [bwa](https://github.com/lh3/bwa). 

Manual scaffolding map created using the [PretextMap](https://github.com/wtsi-hpag/PretextMap) tool. Manual scaffolding performed using the [PretextView](https://github.com/wtsi-hpag/PretextView) tool.

Haplotype 1 is available at [link](https://drive.google.com/file/d/1WbZd9krxL8aP0X-_RRJtyPEjOtB4qrtJ/view?usp=sharing)

Haplotype 2 is available at [link](https://drive.google.com/file/d/17wPcQ5FqNJs018fP9_tMASj5vH2kIc2n/view?usp=share_link)
 
 
| | Haplotype 1 | Haplotype 2 |
|--------|---------|--------|     
| NG50 | 23.244.502 | 25.145.390 |
| # contigs | 370 | 299 |
| Total length | 788.182.177 | 808.327.069 |
| # contigs >= 3Mbp | 32 | 36 |
| Total length* | 703.801.351 | 756.044.094 |
| # contigs* with TR*** at both endings | 7 | 15 |
| # contigs* with TR*** at one of the endings | 13 | 11 |
| # contigs* with no TR*** at the endings | 10 | 10 |
| # contigs >= 1Mbp | 49 | 46 |
| Total length** | 731.151.394  | 773.559.680 |
| # contigs** with TR*** at both endings | 7 | 15 |
| # contigs** with TR*** at one of the endings | 17 | 16 |
| # contigs** with no TR*** at the endings | 25 | 15 |

contigs* - contigs larger or equal to 3Mbp

contigs** - contigs larger or equal to 1Mbp

TR*** - tandem repeats specific for telomeres (ACCCTAA/TTAGGGT)


...

## v0.8


Complete telomere-to-telomere (T2T), gapless assembly (all chromosomes).

Built by integrating hifiasm and Verkko assemblies derived from multiple combinations of input reads (HiFi, UL, etc.).
Scaffolding performed with YAHS.

Additional manual scaffolding using contact maps in Juicebox.

Manual gap filling via local reassembly of HiFi, ultra-long (UL), and HERRO-corrected UL reads.

Haplotype 1 (pat) available at [link](https://drive.google.com/file/d/1RwoCDHIEgFp9yNJ6aOLANt36DMKCv6Ct/view?usp=share_link)

Haplotype 2 (mat) available at [link](https://drive.google.com/file/d/1HSta9GfLQM6JX1XbqEyGGqwSkCw7E9bS/view?usp=sharing)


| | Haplotype 1 (pat) | Haplotype 2 (mat) |
|--------|---------|--------|     
| NG50 | 28Mb | 26MB |
| # chromosomes | 28 | 28 |
| # T2T chromosomes | 28 | 28 |
| Total length | 757.460.232 | 768.943.102 |
| Largest contig | 39.145.193  | 46.917.239 |
| gaps | 0 | 0 |
| GC content (%) | 33 | 33 |
| Genome BUSCOs (%) | 17 | 16 |
| QV | 55 | 50 |


