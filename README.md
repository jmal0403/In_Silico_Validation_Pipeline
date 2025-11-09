# In_Silico_Validation_Pipeline - v.0.0.1

## Summary

### This software provides fully synthetic reads and spike-in reads. 

## Functions:

###  make_ref_fastq(in_num_ref)
### This function provides a FASTQ file with the number of reference (REF) reads to generate as the only input. 
### This set of REF reads are 251 basepairs in length and map to exon 14 of FLT3.

### make_spikein_fastq(in_mut_obj, in_ref_obj, in_num_mut, in_num_ref)
### This function provides a FASTQ file based on a REF SeqRecord object (arg 1) and a MUT SeqRecord objects (arg 2).
### Arg 3 is number of MUTs to add and Arg 4 is the number of total REF seqs.
### For example, the default is 1 Megareads and 10,000 MUT seqs, which provides a 1% VAF.

## Use:

## 1M reference reads
### make_ref_fastq(no_REF)

## 1M reads; 1% VAF; 9bp INS
### make_spikein_fastq(ins_9_SeqRec, ref_record_r1, no_MUT, no_REF)