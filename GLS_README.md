```bash
docker run -itv /data/GL:/data/GL -v /data/GL/database:/database -v .:/workspace namxle/autogvp-tidyverse:4.4.0 bash
```

```bash
cd /workspace && \
Rscript ./scripts/04-filter_gene_annotations.R --vcf results/test_custom.filtered.parsed.tsv --autogvp results/test_custom.custom_input.annotations_report.abridged.tsv --output test_custom --outdir results --colnames ./gvpdata/output_colnames.tsv
```


