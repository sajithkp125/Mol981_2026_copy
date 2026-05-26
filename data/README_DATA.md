---
title: "README_DATA"
author: "Klaus Schliep"
output:
  html_document: default
  pdf_document: default
---

## Data for sequence searches

The file `UndB_sequences.fasta` contains 8 amino acid sequences for the search. Just take the first one for your search, if the program can't fin it try another one. 
These files contain accession numbers from UniProt, here `A4Y0K1` is the accession the first line
`>tr|A4Y0K1|A4Y0K1_ECTM1 Fatty acid desaturase OS=Ectopseudomonas mendocina (strain ymp) OX=399739 GN=Pmen_4370 PE=4 SV=1`.
In case the first accession number does not work try one of the others. 
Also you might find the accession number from NCBI if you blast the sequence and get the best hit. 

[Foldseek](https://search.foldseek.com) can take the UniProt accession number, but you need the database from PDB to AlphaFoldDB. 

## Data for aligning sequences: 

An file with unaligned sequences is: `UndB_unaligned.fasta`
Play around with the gap penalties. 

## Data for ASR

Finally an alignment which can be used for ASR: `UndB_aligned.fasta`

I also added a pre-print of phangorn. Please do not circulate this as not yet submitted. But please tell me if there are spelling mistakes or something is not clear. There is a very short chapter about ASR and I hope you are able to adopt the code from there. 

It needs the development version of `phangorn` installed.  
```
install.packages('phangorn', repos = c('https://klausvigo.r-universe.dev',
                 'https://cloud.r-project.org'))
```
We will use `phangorn` to look at the differences between the methods. 


