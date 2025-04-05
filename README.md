# bugTie 
## bugTie is an Illumina short-read RNAseq analysis pipeline.

Features -
- Low disk footprint by only utilizing gzipped files and directly piping the stdout of HISAT2 into SAMtools.
- Allows for novel isoform detection using the Stringtie suite.
- Generates counts that can be used in the ballgown suite or tools such as DESeq2.
- All in one. Just execute the pipeline and your done; no intermediate pre and post-processing steps. 
- Easily editable and well documented scripts that allow you to update for your needs!

Environment - 
- Be sure that you have conda enabled on your system. 
- To utilize the conda environment activate a new environment in your default envs location with:
`conda env create -f bugTie.yml` 
- Please be aware that this environment is currently still in development. Some packages may be removed upon commiting the final build.

Directory Structure -
```
│   .gitignore # Allows one to ignore our large files (genomes, raw reads, output files, etc.)
│   bugTie_envi.yaml # Allows one to install all required dependencies.
│   README.md # Markdown readme file (this file!)
│   
├───Genome # Stores the genome fasta file, the genome annotation gff file, and some intermediate files such as the Hisat2 index.
│       genomeReadMe.txt
│
├───Output # This directory holds the output files. It will have subdirectories according to each step in the pipeline.
│       outputReadMe.txt
│
├───RawData # This directory holds our .fq.gz files.
│       rawdataReadMe.txt
│
└───Scripts # This directory stores our scripts.
        scriptsReadMe.txt
```