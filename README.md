# How to make pot-files for PE calculations

- All the scripts used can be cloned from here:
```sh
git clone git@github.com:arnfinn/scripts.git
```

## Get xyz-files from a pdb-file

```sh
./pdb-prep.py --split filename.pdb # It seems like I have not implemented this feature yet...
```

## Make the MolCas input files

```sh
./subloprop -xyz filename.xyz
```

## Run MolCas on Stallo

```sh
module load molcas
```


