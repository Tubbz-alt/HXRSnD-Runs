======================
Archive of HXRSnD Runs
======================

This repo serves as the working directory of each HXRSnD run and as an archive
of previous runs.

Basic Usage
-----------

Alignments are performed by running the ``run_snd_notebook`` script, which will
set up the environment and launch the notebook. Changes to the run setup should
only be done in this notebook template. Snapshots of the notebook can be made
using the ``archive`` script.

Notebook Archive
----------------

Previous runs are in directories named by the date the alignment was run, and
the files themselves are named using the template name, date and time it was
saved.

Adding Sanpshots
----------------

To create a snapshot of the template notebook, simply run the ``archive``
script, ::

  ./archive

A new file should be added that has the directory and name structure mentioned
above. If the desired notebook to be archived is not the standard template
notebook, then the path can be specified as follows: ::

  ./archive --template <<path_to_file>>

The script takes additional arguments if slight deviations of the
general work-flow is needed. Valid arguments are:

    -h, --help           show this help message and exit
    -v, --verbose        Increase verbosity.
    -d, --debug          Run in debug mode.
    --log_dir P          Path to save the logs in.
    -t P, --template P   Template file path to be copied.
    -s P, --save_path P  Save path for copied file.
