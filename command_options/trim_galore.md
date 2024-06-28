# Trim Galore Command

```
trim_galore
  --cores 4
  --paired
  --gzip
  --output_dir output_dir
  -a AGATCGGAAGAGC
  -a2 AAATCAAAAAAAC
  trim_galore_input_file_read1
  trim_galore_input_file_read2
```

### Notes
- **output_dir**: Directory labeled "trim_galore_output" in each sample RS folder - generated with code in the main Pipeline file.
- **trim_galore_input_file_read1**: FASTQ file in each RS folder ending with R1_001.fastq.gz.
- **trim_galore_input_file_read2**: FASTQ file in each RS folder ending with R3_001.fastq.gz.

*R2_001 omitted because it is used as an index during deduplication.*
