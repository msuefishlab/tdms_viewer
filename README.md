# tdmsviewer

[![Build Status](https://travis-ci.org/msuefishlab/tdmsviewer.svg?branch=master)](https://travis-ci.org/msuefishlab/tdmsviewer)

Programs for seeking and analyzing LabVIEW tdms files

## Install


    install.packages('devtools')
    devtools::install_github('msuefishlab/tdmsviewer')

## Run server


    library(tdmsviewer)
    # basedir defaults to ~/
    # the directory selector can look for tdms files in this subtree
    tdmsviewer(basedir='~/tdms_files')

## Usage

Navigate to the webpage, and choose a directory that contains TDMS files using the "Directory select" button to load the files in that directory into a dropdown box

To interact with the TDMS data, you can use the following tools

- Use the plus and minus buttons to zoom in and out
- The range slider allows you to select the start and end of the range you want to view
- Click and drag the mouse over the plot of the data itself to zoom in on a region

## Screenshot

![](img/1.png)


## Documentation

The markdown vignette which includes installation instructions and user manual is available at <https://msuefishlab.github.io/tdmsviewer/>


## Notes

Based on the [tdmsreader](https://github.com/msuefishlab/tdmsreader) package
