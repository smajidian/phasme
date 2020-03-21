PhaseME
======

PhaseME is a tool set to assess the quality of the per read phasing information and help to reduce the errors during this process. 


# Quickstart

1- You require your VCF file to be read based phased, which can be generated by e.g. WhatsHap.

2- Run PhaseME to obtain stats and improve the quality of phase blocks.

```
python phaseme.py improver my.vcf precomputed
```
If you only want to have QC report use `qc` instead of `improver`. 


## Installation Test

Please try our sample data to establish the correctness of the pipeline installation. This can be found in the folder `example`.




## Individual-specific linkage information

For grasping the full advantage of PhaseME, few steps needed prior using PhaseME.

1- You need 1000 Genomes reference panel haplotypes, which can be obtained from [here](https://mathgen.stats.ox.ac.uk/impute/1000GP_Phase3.html)

```
wget https://mathgen.stats.ox.ac.uk/impute/1000GP_Phase3.tgz

wget https://mathgen.stats.ox.ac.uk/impute/1000GP_Phase3_chrX.tgz
```

Warning: These are more than 10Gb.


2- You need to download the [Shapeit](https://mathgen.stats.ox.ac.uk/genetics_software/shapeit/shapeit.html)

3- Now run the following


```
python phaseme.py improver my.vcf /path/to/shapeit
```




# Citation:

Please see and cite our manuscript: "PhaseME: automatic assessment of phasing quality and phasing improvement"






