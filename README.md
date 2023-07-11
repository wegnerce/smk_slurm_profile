
# smk_slurm_profile
This is my current [`Snakemake`](https://snakemake.github.io/) profile that I use with the HPC infrastructure of the Friedrich Schiller University Jena, which relies on [`SLURM`](https://slurm.schedmd.com/overview.html).

I shamelessly copy&pasted the profile from [Michael Roachs' blog post](https://fame.flinders.edu.au/blog/2021/08/02/snakemake-profiles-updated). 

While reading about `Snakemake` profiles I found the following links particularly useful:
> * https://fame.flinders.edu.au/blog/2020/09/04/snakemakeprofile
> * https://fame.flinders.edu.au/blog/2021/08/02/snakemake-profiles-updated
> * https://bluegenes.github.io/Using-Snakemake_Profiles/

`Snakemake` profiles are available from the [Snakemake-profiles project](https://github.com/Snakemake-Profiles/doc). The `SLURM`profile is maintained by [@percyfal](https://github.com/percyfal) and makes use of [`cookiecutter`](https://github.com/cookiecutter/cookiecutter).
## Usage
```bash
# 1 | download the profile
# 2 | copy it to the config folder
# 3 | make the slurm_status.py script executable
git clone https://github.com/wegnerce/smk_slurm_profile.git
cp -r smk_slurm_profile/* ~/.config/snakemake/slurm/
chmod +x ~/.config/snakemake/slurm/

# run snakemake with the profile
snakemake --profile slurm
```

:copyright: Carl-Eric Wegner, 2023
