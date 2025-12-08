### AmpWrap Analysis
Visit: https://github.com/LDoni/AmpWrap  
and follow the instructions provided in the repository to run the complete analysis.

### Reviewing the Results
#### 1. Initial Quality Control with FastQC and Summary Report with MultiQC

Navigate to the `raw_qc_initial` directory:
   ```
   cd run_1/QC/raw_qc_initial
   ls -ltrh
   ```
   Examine the generated files. Opening a FastQC HTML report will display a detailed assessment of raw read quality, including per-base quality scores, sequence length distribution, GC content, and other key metrics.

   The MultiQC HTML report provides an aggregated, sample-wide overview of all FastQC outputs, enabling a comparative evaluation of sequencing quality across the dataset.
   
   FastQC documentation: https://www.bioinformatics.babraham.ac.uk/projects/fastqc/Help/3%20Analysis%20Modules/
   
   MultiQC tutorial: https://www.youtube.com/watch?v=qPbIlO_KWN0

#### 2. Primer removal from sequencing reads with Cutadapt.


#### 3. Post-cutadapt quality control with FastQC and QC report generation with MultiQC
   After primer trimming, FastQC and MultiQC are run again to evaluate improvements in read quality and to verify the effectiveness of the trimming step.
   Navigate to the `raw_qc_post_cutadapt` directory:
   ```
   cd run_1/QC/raw_qc_post_cutadapt
   ls -ltrh
   ```
#### 4. Determine optimal trimming parameters for DADA2 with FIGARO
#### 5. Amplicon sequence variant inference with DADA2
   - Filter and trim
     AmpWrap implements the automation of trimming parameters for DADA2 denoising using FIGARO
   DADA2 tutorial: https://benjjneb.github.io/dada2/tutorial.html
