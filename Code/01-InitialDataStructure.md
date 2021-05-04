# `01-InitialDataStructure.md`

Downloading, inspecting, and describing the data utilized in the study.

Updated by Marissa on April 29, 2021.

## Software & Packages used in this study

* sra-toolkit (LINK)
* trim_galore (LINK)
* bowtie2 (LINK)
* TSAS (LINK)
* MochiView?? (LINK)
* R (LINK)
* R studio (LINK)
* 	ggplot??? others?



## Sequence Read Archive (SRA) files

### Downloading files

I downloaded 4 files from the Sequence Read Archive on April 14, 2021: `SRR13258538`, `SRR13258539`, `SRR13258540`, `SRR13258541`. Using the `sra-toolkit` package downloaded from [NCBI on GitHub](https://github.com/ncbi/sra-tools/wiki), the files were converted into FASTQ format.      



### General information about the files:

**File Name, Experiment Accession, Sample Accession, Total Bases, and Library Name**

* **SRR13258538**, SRX9689339, SRS7886629, 41705709 bases, E3_enrichment
* **SRR13258539**, SRX9689338, SRS7886628, 48172356 bases, E2_enrichment
* **SRR13258540**, SRX9689337, SRS7886627, 43481631 bases, E1_enrichment
* **SRR13258541**, SRX9689336, SRS7886626, 34329120 bases, Library

### File dimensions

	wc SRR13258538.fastq SRR13258539.fastq SRR13258540.fastq \
		SRR13258541.fastq

	Lines		Words		Characters		File name
	3271036 	6542072 	145116682 		SRR13258538.fastq
	3778224 	7556448 	167686548 		SRR13258539.fastq
	3410324 	6820648 	151314998 		SRR13258540.fastq
	2692480 	5384960 	119370940 		SRR13258541.fastq

### File size

	du -h SRR13258538.fastq SRR13258539.fastq SRR13258540.fastq \
		SRR13258541.fastq
			
	144M	SRR13258538.fastq
	161M	SRR13258539.fastq
	160M	SRR13258540.fastq
	128M	SRR13258541.fastq

### Number of rows of data 
There are 4 rows of data per entry. Each entry starts with @FILENAME, so counting this for each file gives an accurate number of entries. This is equal to the number of lines divided by four.

	grep "^@SRR13258538" SRR13258538.fastq | wc -l		817759
	grep "^@SRR13258539" SRR13258539.fastq | wc -l 		944556
	grep "^@SRR13258540" SRR13258540.fastq | wc -l 		852581
	grep "^@SRR13258541" SRR13258541.fastq | wc -l 		673120
	
	
## *Pseudomonas aeruginosa* MPAO1 genome & annoation files

### Downloading files

...

### File dimensions
...

### File size

...


## Supplementary material data tables

### Downloading files

...

### File dimensions
...

### File size

...