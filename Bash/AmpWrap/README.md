### AmpWrap Analysis
Visit: https://github.com/LDoni/AmpWrap  
and follow the instructions provided in the repository to run the complete analysis.

### Reviewing the Results

1. Initial quality control with FastQC and QC report generation with MultiQC

MultiQC tutorial: https://www.youtube.com/watch?v=qPbIlO_KWN0

2. Primer removal from sequencing reads with Cutadapt. The --discard-untrimmed option is applied
3. Post-cutadapt quality control with FastQC and QC report generation with MultiQC
4. Determine optimal trimming parameters for DADA2 with FIGARO
5. Amplicon sequence variant inference with DADA2
   
