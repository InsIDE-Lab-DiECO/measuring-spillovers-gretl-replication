# measuring-spillovers-gretl-replication
Replication package for “Measuring spillovers and connectedness in gretl” by Chiara Casoli and Luca Pedini (Computational Statistics, 2026).

HOW TO INSTALL DYconn AND REPLICATE THE EXERCISE

IMPORTANT: To replicate the results in this exercise, you must use the
version of DYconn provided in the accompanying ZIP file. The version
currently available in the official gretl repository may change in the
near future and may not reproduce the reported results.

The DYconn package is also available in the official gretl online
repository. To install that version, type in a gretl console:

    ? pkg install DYconn

or use the GUI via:
    File → Function packages → On server → DYconn

WARNING: The repository version corresponds to DYconn v0.1 and may be
updated in future releases. For replication purposes, we do not recommend to rely on the
repository version.

1. MANUAL INSTALLATION (RECOMMENDED FOR REPLICATION)

To install the exact version used in this exercise, open a gretl console
and type:

    ? pkg install /path/to/local/DYconn.zip --local

Replace "/path/to/local/" with the actual directory where DYconn.zip is located.

2. RUNNING THE REPLICATION SCRIPT

To replicate the exercise, simply run the following script:

    CS_replication.inp

3. NOTES

-- 3.1: The bootstrap procedures — especially the one involving dynamic connectedness — are time- and CPU-intensive. You may want to run them separately.

-- 3.2: If you prefer NOT to install the package but still want to use it:
  - Unzip DYconn.zip
  - Extract the following files:
      - DYconn.gfn
      - dy2009.gdt (from the "example" folder)
  - Place all these files in the same directory together with CS_replication.inp.
  - Open CS_replication.inp in gretl, and simply remove or comment --frompkg=DYconn
    from the open command line.


## DOI

This replication package is archived at Zenodo:

[10.5281/zenodo.18592749](https://doi.org/10.5281/zenodo.18592749)
