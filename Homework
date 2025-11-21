#!/bin/sh
#I set the directory back to the environment from class
cd ~/PBC450_2025/soil_metagenomics/20251107_1254_MN29288_FBE86142_e0306a7f/pod5/demux/
#I ran the NanoPlot for Barcode 20
NanoPlot -o barcode20_np --fastq e0306a7f-0f47-436a-bfef-23e64d0532f5_SQK-RBK114-24_barcode20.fastq
#I opened a new terminal to move the files for barcode 20 onto my laptop
scp -r snq7572@10.2.0.53:/home/snq7572/PBC450_2025/soil_metagenomics/20251107_1254_MN29288_FBE86142_e0306a7f/pod5/demux/barcode20_np .
#I ran epi2me wf-metagenomics pipeline on barcode 20 data using nextflow
nextflow run epi2me-labs/wf-metagenomics --fastq e0306a7f-0f47-436a-bfef-23e64d0532f5_SQK-RBK114-24_barcode20.fastq --out_dir barcode20_metagen
#Then I ran next scp on my laptop, saving barcode 20 to my laptop
scp -r snq7572@10.2.0.53:/home/snq7572/PBC450_2025/soil_metagenomics/20251107_1254_MN29288_FBE86142_e0306a7f/pod5/demux/barcode20_metagen .
