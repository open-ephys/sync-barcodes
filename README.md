# Sync Barcodes

This repository contains Arduino code (`arduino-barcodes`) for generating TTL barcodes that can be used to synchronize various data sources.

First, the output pin of the Arduino must be connected to a digital input line of all devices with independent clocks. Once acquisition is finished, the unique 32-bit barcodes can be used to align the data offline, even if one of the data streams is interrupted during the experiment. 

`barcodes.py` provides an example of how to extract the barcode values from an array of on/off events.

## Alternative implementation

For a better documented, more rigorously validated version of the sync barcodes concept, check out the [DAQ Synchronization Project](https://optogeneticsandneuralengineeringcore.gitlab.io/ONECoreSite/projects/DAQSyncro/BarcodeGeneration/) from the [Optogenetics and Neural Engineering Core](https://optogeneticsandneuralengineeringcore.gitlab.io/ONECoreSite/) at the University of Colorado Denver.
