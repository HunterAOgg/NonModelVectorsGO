This repository contains a few custom libraries containing GO annotations and mappings between gene symbols and gene IDs for non-model organisms that are vectors of infectious diseases.

These are intended primarily to facilitate gene-set enrichment analysis. All annotations were created using EGG-NOG. For Culicidae (mosquito) species, homology was restricted to diptera (7147).
For Chiroptera (bat) species, homology was not restricted. Otherwise, the details for the command usage were the same as below.

## emapper-2.1.12
## /data/shared/home/emapper/miniconda3/envs/eggnog-mapper-2.1/bin/emapper.py --cpu 20 --mp_start_method forkserver --data_dir /dev/shm/ -o out --output_dir /emapper_web_jobs/emapper_jobs/user_data/MM_6t2_c4rq --temp_dir /emapper_web_jobs/emapper_jobs/user_data/MM_6t2_c4rq --override -m diamond --dmnd_ignore_warnings -i /emapper_web_jobs/emapper_jobs/user_data/MM_6t2_c4rq/queries.fasta --evalue 0.001 --score 60 --pident 40 --query_cover 20 --subject_cover 20 --itype CDS --translate --tax_scope 7147 --target_orthologs all --go_evidence all --pfam_realign none --report_orthologs --decorate_gff yes --excel
