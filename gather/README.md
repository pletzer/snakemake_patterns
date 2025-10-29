# Gather pattern

This example runs tasks a, b and c. These produce files a.txt, b.txt and c.txt, respectively. Task c can only be run once tasks a and b have successfully completed.

To run the example, type
```bash
snakemake -j 2
```
You should now see the files `a.txt`, 'b.txt` and 'c.txt` being created. 