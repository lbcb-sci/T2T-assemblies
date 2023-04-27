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

Haplotype 1 is available at [link](https://durianreferencelbcb.s3.eu-central-1.amazonaws.com/durian.hifiasm.hic.ulont100.asm.hic.hap1.p_ctg.fa)

Haplotype 2 is available at [link](https://durianreferencelbcb.s3.eu-central-1.amazonaws.com/durian.hifiasm.hic.ulont100.asm.hic.hap2.p_ctg.fa)
 
 
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

### D-Genies plots - assemblies vs reference
![](https://github.com/lbcb-sci/T2T-assemblies/blob/main/data/v0.1-assembly-to-reference.png)
 
## v0.2

The assembly was created using [hifiasm](https://github.com/chhylp123/hifiasm) utilizing Hi-C reads to produce a phased diploid assembly.

Haplotype 1 is available at [link](https://durianreferencelbcb.s3.eu-central-1.amazonaws.com/hifiasm_err_corr_100k_nochim.asm.hic.hap1.p_ctg.fa)

Haplotype 2 is available at [link](https://durianreferencelbcb.s3.eu-central-1.amazonaws.com/hifiasm_err_corr_100k_nochim.asm.hic.hap2.p_ctg.fa)

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


### D-Genies plots - assemblies vs reference
![](https://github.com/lbcb-sci/T2T-assemblies/blob/main/data/v0.2-assembly-to-reference.png)

## v0.3

The results of the first rounds of manual scaffolding using assembly v0.2. 

For manual scaffolding HiC reads were mapped to assembly using [bwa](https://github.com/lh3/bwa). 

Manual scaffolding map created using the [PretextMap](https://github.com/wtsi-hpag/PretextMap) tool. Manual scaffolding performed using the [PretextView](https://github.com/wtsi-hpag/PretextView) tool.

Haplotype 1 is available at [link](https://durianreferencelbcb.s3.eu-central-1.amazonaws.com/hap1.scaffolds.fasta)

Haplotype 2 is available at [link](https://durianreferencelbcb.s3.eu-central-1.amazonaws.com/hap2.scaffolds.fasta)
 
 
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


### D-Genies plots - assemblies vs reference

![](https://github.com/lbcb-sci/T2T-assemblies/blob/main/data/v0.3-durian-assembly-to_reference.png)

## v0.4

ULONT data was utilized for scaffolding with the [SAMBA](https://github.com/alekseyzimin/masurca) scaffolder.

Haplotype 1 is available at [link](https://ferhr-my.sharepoint.com/:u:/g/personal/ftomas_fer_hr/Eaywgjh-HOJBmwC1HNWZWKcBHl3NdZdrskR4R8hSadFOsA?e=K54txv)

Haplotype 2 is available at [link](https://ferhr-my.sharepoint.com/:u:/g/personal/ftomas_fer_hr/Ee1cKlTiCKxIrwqu79AjYL0BAOvHtsb1af9VzJc-i_GWDQ?e=1VSznl)

 
| | Haplotype 1 | Haplotype 2 |
|--------|---------|--------|     
| NG50 | 22.234.587 | 23.157.154 |
| # scaffolds | 349 | 309 |
| Total length | 791.086.597 | 802.879.292 |
| # scaffolds >= 3Mbp | 40 | 39 |
| Total length* | 731.545.803 | 791.086.597 |
| # scaffolds* with TR** at both endings | 14 | 15 |
| # scaffolds* with TR** at one of the endings | 24 | 21 |
| # scaffolds* with no TR** at the endings | 2 | 3 |

scaffolds* - scaffolds larger or equal to 3Mbp

TR** - tandem repeats specific for telomeres (ACCCTAA/TTAGGGT)


### D-Genies plots - assemblies vs reference
![](https://github.com/lbcb-sci/T2T-assemblies/blob/main/data/v0.4-durian-assembly-to_reference.png)
