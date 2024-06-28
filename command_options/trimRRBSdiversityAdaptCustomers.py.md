# NuGEN Diversity Trimming Command
```
python2
trimRRBSdiversityAdaptCustomers.py
  -1 nugen_input_file_read1
  -2 nugen_input_file_read2
  -o output_dir
```
### Notes
- **python2:** Specifying python 2 because this script runs using that version of python
- **nugen_input_file_read1:** Contains read 1 fastq file generated after trim galore trimming in trim_galore_output directory
- **nugen_input_file_read2:** Contains read 2 fastq file generated after trim galore trimming in trim_galore_output directory
- **output_dir:** Contains a file path to a directory for trimming outputs in each RS folder. *May not be functional, further investigation needed*
