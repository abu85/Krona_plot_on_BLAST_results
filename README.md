# Krona_plot_on_BLAST_results
## 1. Load Krona modules or softwares
- In local computer: https://github.com/marbl/Krona/wiki/Installing
- In server (e.g. uppmax) run this: 
`module load bioinfo-tools Krona/2.7`

## 2. Krona main command and explanation

`ktImportTaxonomy 
GT48_blast_results.txt 
-o Krona_GT48_blast_results.html 
-t 4 
-s 3 
-q 1`

### Explanation: 
- `ktImportTaxonomy` = main command
- `BLAST_OUTPUT_FILE` = BLAST results file, the file contain BLAST output, use this this file as input, this file should contain taxid column
- `-o` `KRONA_PLOT.html` = Krona output,  KRONA_PLOT.html is file, this will be creted after running the command
- `-t` `4` = taxonomic ID column, here number 4 is the taxid column in my blast output file 
- `-s` `3` = score column, here number 3 is the score column in my blast output file
- `-q` `1` = query IDs column, here number 1 is the query column in my blast output file

details explanation can be found here http://manpages.ubuntu.com/manpages/impish/man1/ktImportTaxonomy.1.html

## END
