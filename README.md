# tdmsviewer

Programs for seeking and analyzing LabVIEW tdms files

## Install


    install.packages('devtools')
    devtools::install_github('msuefishlab/tdmsviewer')

## Run server


    library(tdmsreader)
    tdmsreader()

## Usage

Navigate to the webpage, and choose a directory that contains TDMS files using the "Directory select" button to load the files in that directory into a dropdown box

To interact with the TDMS data, you can use the following tools

- Use the plus and minus buttons to zoom in and out
- The range slider allows you to select the start and end of the range you want to view
- Click and drag the mouse over the plot of the data itself to zoom in on a region

## Screenshot

![](img/1.png)


## Notes

When installing on Windows, the dependencies are not fully completed by the `install_github` step, so perform this step prior to `install_github('msuefishlab/tdmsviewer')`

    install.packages(c('shiny','RJSONIO'))

By default, the baseDir is the home directory '~' but you may find, for example, on Windows, that you can run

    tdmsviewer::tdmsviewer(baseDir = '~/..')

This gives access to Downloads folder, Desktop, etc.
