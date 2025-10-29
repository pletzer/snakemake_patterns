# Slurm parametrized gather pattern

This example runs a set of tasks prep{idx}. Task final can only be run once tasks prep{idx} have successfully completed. The prep tasks are submitted using the scheduler (SLURM). The last task, final, is executed interactively. 

To run the example, type
```bash
snakemake -j 8 --cluster "sbatch -t 00:01:00 --ntasks=2 --hint=multithread --mem=2G"
```
You should now see the files `prep*.txt` and 'final.txt` being created. 