# How to make pot-files for PE calculations

All the scripts used can be cloned from here:
```
git clone git@github.com:arnfinn/scripts.git
```

## Get xyz-files from a pdb-file

```
pdb-prep.py --split filename.pdb # It seems like I have not implemented this feature yet...
```

## Make the MolCas input files

```
subloprop -xyz filename.xyz
```

## Run MolCas on Stallo

```
module load molcas
molcas filename.inp
```

This will produce a file named filename.MpProp

## Make pot-file out of MpProp-file(s)

```
MpProp2pot.py -i filename(s).MpProp -o filename.pot
```




