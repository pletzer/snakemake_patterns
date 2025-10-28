# Gather pattern

This example runs a set of tasks prep{idx}. Task final can only be run once tasks prep{idx} have successfully completed.

To run the examples, type
```bash
snakemake -j 8
```
You should now see the files `prep*.txt` and 'final.txt` created. 