This folder contains the research on the H-bond - chemical shift relationships

# Statistical data 

## Relation of PDB and BMRB

`PDB_BMRB_pairs.csv`

## The dataset
The file `shifts_H-bond_lens_DSSP_PDBs_neighbors.zip` contains a tab-separated table (`*.tab`) that relates chemical shift and H-bond information. 
Definitions

| Column name | Description                                                                                            |
|-------------|--------------------------------------------------------------------------------------------------------|
| PDB_ID      | The PDB ID                                                                                             |
| BMRB_ID     | The BMRB ID                                                                                            |
| CHAIN       | Chain name - only chains 'A'!                                                                          |
| #           | Number of the residue in the sequence                                                                  |
| AA          | One-letter amino acid code                                                                             |
| Comp_ID     | Three-letter amino acid code                                                                           |
| SS          | Secondary structure: either E or B                                                                     |
| prev_type   | Three-letter code of residue i-1                                                                       |
| next_type   | Three-letter code of residue i+1                                                                       |
| PHI         | Phi angle (determined with DSSP)                                                                       |
| PSI         | Psi angle (determined with DSSP)                                                                       |
| NH-OX_idx   | Number of H-bond acceptor residue (by DSSP); X takes 1 and 2                                           |
| NH-OX_En    | Energy of the H-bond between the query residue and the acceptor (by DSSP); X takes 1 and 2             |
| O-NHX_idx   | Number of H-bond donor residue (by DSSP); X takes 1 and 2                                              |
| O-NHX_En    | Energy of the H-bond between the query residue and the donor (by DSSP); X takes 1 and 2                |
| H_bond_X    | Length of the H-bond where the query resiue is donor. Measured from the PDB file. X takes 1 and 2      |
| H_bond_XX   | Length of the H-bond where the query resiue is acceptor. Measured from the PDB file. X takes 1 and 2   |
| H_bond_min  | Length of the shortest of the four H-bonds identified by DSSP                                          |
| O_Y         | Number of the residue containing an oxygen within 3.9 Angstrom from the N of the query residue. Y takes from 1 to 4 |
| NO_len_Y    | Length between the nitrogen of the query residue and the oxygen Y. Y takes 1 to 4.                     |
| Atom_ID     | Atom name. Takes HN, N, CA or CB                                                                       |
| Val         | Chemical shift                                                                                         |
