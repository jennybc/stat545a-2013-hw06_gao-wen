README
========================================================



How to replicate my analysis

  * Clone the repo!
  * Download into an empty directory:
    - Input data: [`lotr_raw.tsv`](data/clean_globalterrorismdb_1012dist.tsv). This file is modified from the original data by removing unnecessary text columns, so it won't give error when loading into R.
    - Scripts: [`dataPrep.r`](dataPrep.r) and [`plotByGroup.r`](plotByGroup.r)
    - Makefile-like script: [`Makefile.r`](Makefile.r)
  * Start a fresh RStudio session, make sure the above directory is the working directory, open `Makefile.r`, and click on "Source".
  * Alternatively, in a shell: `Rscript Makefile.r`.
  * When you run the pipeline the first time, you will get warnings about `file.remove()` trying to remove files that don't exist. That's OK. They will exist and will be removed and remade on subsequent runs.
  * New files you should see after running the pipeline:
