# Bismark Command
```
bismark
  --bowtie2
  --gzip
  --bam
  --p 20
  --genome_folder genome_dir
  -1 bismark_input_file_read1
  -2 bismark_input_file_read2
  --outdir output_dir
```
### Notes
- **genome_dir:** is a file path to a directory containing a reference genome fasta file (.fa) and annotation file (.gtf)
- **bismark_input_file_read1:** Contains read 1 fastq file generated after NuGEN trimming in nugen_trim_output directory
- **bismark_input_file_read2:** Contains read 2 fastq file generated after NuGEN trimming in nugen_trim_output directory
- **output_dir:** Contains a file path to a directory for alignments in each RS folder
