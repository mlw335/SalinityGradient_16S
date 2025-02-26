# code to execute fastqc

  352  fastqc /workdir/mlw335/SalinityGradient_16S/data/01_DADA2/01_raw_gzipped_fastqs/*.fastq.gz --threads 5 -o /workdir/mlw335/SalinityGradient_16S/analysis/00_FastQC/fastqc_reports/

# code to execute multiqc

  370  multiqc fastqc_reports/ -o multiqc_results/

# load multi/fast qc
  293 export PATH=/programs/FastQC-0.12.1:$PATH
  294  export PYTHONPATH=/programs/multiqc-1.15/lib64/python3.9/site-packages:/programs/multiqc-1.15/lib/python3.9/site-packages
  295  export PATH=/programs/multiqc-1.15/bin:$PATH
