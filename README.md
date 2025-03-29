# bugTie 
## bugTie is a Illumina short-read RNAseq analysis pipeline.

Features -
- Low disk footprint by only utilizing gzipped files and directly piping the stdout of HISAT2 into SAMtools.
- Allows for novel isoform detection using the Stringtie suite of tools.
- Generates counts that can be used in the ballgown suite or tools such as DESeq2.
- All in one. Just execute the pipeline and your done; no intermediate pre and post-processing steps. 
- Easily editable and well documented scripts that allow you to update for your needs!

Environment - 
- Be sure that you have conda enabled on your system. 
- To utilize the conda environment activate a new environment in your default envs location with:
`conda env create -f bugTie.yml` 
- Please be aware that this environment is currently still in development. Some packages may be removed upon commiting the final build.