
Requirements
```bash
conda create -n legolas python=3.8
conda install -c https://roitberg.chem.ufl.edu/projects/conda-packages-uf-gainesville -c pytorch -c nvidia -c defaults -c conda-forge sandbox
pip install pkbar tensorboard tqdm matplotlib biopython pandas
```

Run
```bash
# atypes = HA, H, CA, CB, C, N
python run.py {pdb_file}
```

Example
```bash
python run.py data/304temp.pdb
python run.py data/304temp.pdb -atype H,C,N
python run.py data/304_BBL.nc -t data/304_BBL.parm7
```
