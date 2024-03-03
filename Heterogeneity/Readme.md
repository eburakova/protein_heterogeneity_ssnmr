# A collection of \*.ipynb related to the main PhD project

## Content description

* Linewidths measurements in 3D
    - Line widths - based metrics of heterogeneity

* Hydrophobin analysis with TALOS
    - TALOS approach illustrated on for EASd15
    - The approach has been published in *Burakova et al, J. Biomol. NMR, 2022*

## Setup

* Make sure that Python is installed and is in `$PATH`.
* Download PACSY database at http://pine.nmrfam.wisc.edu/download_packages.html. It is mostly required for plots and for the detailed analysis but is not strictly necessary for the "TALOS approach".  
* Have your processed 4D hCBCANH at hand.

For `Windows`: 

open `PowerShell` CLI as an administrator:

```powershell
pyenv local 3.11.3
python -m venv .venv
.venv\Scripts\Activate.ps1
python -m pip install --upgrade pip
pip install -r requirements
```

For `Linux` or `macOS`:

```bash
pyenv local 3.11.3
python -m venv .venv
source .venv/bin/activate
pip install --upgrade pip
pip install -r requirements
```

Download PACSY to the repo root directory and run the following commands:
> if you use Windows, open a Bash terminal with `GitBash` or WSL.
```bash
unzip pacsy_csv.zip
cp zavot/data/whlee/pacsy/CSV_042822/*_DB2.txt ./data/pacsy/
cp zavot/data/whlee/pacsy/CSV_042822/CS_STATS_DB.txt ./data/pacsy/
```
