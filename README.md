# ssRNA-sequencing-code-
#install SRA tool kit
wget --output-document sratoolkit.tar.gz https://ftp-trace.ncbi.nlm.nih.gov/sra/sdk/current/sratoolkit.current-ubuntu64.tar.gz
#prefetch PRJNA416930
#fasterq_dump
#Download Mus_musculus.GRCm39.dna.primary_assembly.fa and Mus_musculus.GRCm39.111.gtf from ensembel
# Alignment
STAR --runThreadN 6 --runMode genomeGenerate --genomeDir ~/SsRNA/INDEX/ --genomeFastaFiles Mus_musculus.GRCm39.dna.primary_assembly.fa --sjdbGTFfile Mus_musculus.GRCm39.111.gtf --sjdbOverhang 90


