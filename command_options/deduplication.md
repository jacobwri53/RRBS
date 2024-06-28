# 4 Step Deduplication Workflow

## 1. Generate SAM files from BAM files
- *Needed for NuGEN custom stripping script*

```
samtools view
-o output_sam_file
-h
bam_file
```
### Notes
- **output_sam_file:** Contains a file path to a SAM file to be written
- **bam_file:** Contains a file path to a BAM file to be converted to output_sam_file

## 2. Custom Bismark Stripping Script
- *Required for Tecan Deduplication script*

```
./strip_bismark_sam.sh
sam_file
```
### Notes
- **strip_bismark_sam.sh** script *MUST* be in the same directory as the Jupyter Notebook
- **sam_file:** Contains a file path to the SAM file generated in the previous step

## 3. Deduplication
- *Using custom script from Tecan*

```
./nudup.py
-2
-f read_file
-o output_file
sam_file
```
### Notes
- **nudup.py** script *MUST* be in the same directory as the Jupyter Notebook
- **read_file:** Contains a file path to an index file supplied by core - *From Roswell GSR this is R2_001 (Original read file)*
- **output_file:** Contains a file path to an outputted *BAM* file located in each RS folder, marked up, deduplicated, and log

## 4. Remove Generated SAM Files
- No custom script, does not remove any non-SAM files
  - Although it may not be useful, marked up BAM file is not removed yet
