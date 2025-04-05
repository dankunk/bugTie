# Metadata file
This file is a tab delimited text file that is passed as a command line argument when running the execute script.

This document should have no headers. 
An example first line of this file would have the structure of:

Read1   Read2   GS+Count    Count_treat_sampleID treat biorep#   

T1_2_1.fq	T1_2_2.fq	RP01	01_zt4_2	zt4	1

Read1 = First/Forward read.

Read2 = Second/Reverse read.

GS+Count = This is a unique ID combining the genus and species initials and a counter for each sample regardless of treatment group.
    For instance if there were 30 samples total, the last row for this column would read RP30.
    Samples will be processed and placed into directories according to this value.

Count_treat_sampleID = This is another unique ID combining a few identifiers.
    This