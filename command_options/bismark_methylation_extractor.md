# Bismark Methylation Exctractor Command

```
bismark_methylation_extractor
--paired-end
--comprehensive
--merge_non_CpG
--output_dir output_dir
--gzip
--parallel 15
--bedGraph --remove_spaces
--cytosine_report
--genome_folder genome_dir
```
### Notes
- **Comprehensive** mode used to merge all strands together
- **merge_non_CgP** mode used to merge CHG and CHH contexts together to have fewer extra files
- **bedGraph** mode used to produce a Bed Graph file (not sure if this will be necessary yet)
- **Cytosine Report** mode used to produce a report of cytosine methylation contexts and statistics (not sure if this will be necessary yet)
- **output_dir:** Contains a file path to a directory in the *RQ* folder (not individual to RS folders)
- **genome_dir:** is a file path to a directory containing a reference genome fasta file (.fa) and annotation file (.gtf)
