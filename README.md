# ECMWF_MJO-QBO
Holds data files from MJO-QBO connection experiments conducted at ECMWF in support of the paper 
"The impact of the stratosphere on the MJO in a forecast model" submitted publication pending to 
the Journal of Geophysical Research - Atmospheres.

This repository contains processed output from the original experiments which were used in creating the figures and analysis
which comprised the final publication. The folders are:

January01_tu_composites:

Temperature and wind composites from all experiments initialized on January 1. The temperature files are 
denoted "t" and the wind are "u". The labels "ctrl", "QE", or "QW" indicate respectively whether the file was taken from a run
with the observed stratosphere, the imposed QBOE stratosphere, or the imposed QBOW stratosphere as defined in the paper.

Phase2_tu_composites & Phase4_tu_composites:

As in the above, but for (respectively) the experiments initialized when the MJO is strong and in Phase 2 or strong and in 
Phase 4 (respectively). Here no control is run and hence not provided.

RMM_ctrlclim:

The RMM values for each simulation -- here RMM is calculated relative to the "control climatology" as opposed to the
"QBO climatology" -- please refer to the paper for more informattion. The subfolders "January 01", "Phase2" and "Phase4" 
distinguish as above the initialization dates.

All files begin with the initialization date of the form YYYYMMDD or in the case of the January01 files simply YYYY.

RMM1 or RMM2 then refers to which principal component of the index is calculated.

Finally the endings are "obs" -- observations; "ctrl" -- control simualtion; "QE" -- imposed-QBOE; "QW" -- imposed-QBOW.

ROMI_ctrlclim:

Largely idential to the RMM file structure. The only exception is for the "January01" files individual years are combined into
simple files, with the labels as follows: "ctrl" -- control simulation; "verif" -- observed; "eqbo" -- imposed QBOE; "wqbo" -- 
imposed QBOW. Within those files the individual ROMI1 and ROMI2 files are saved.

Appendix:

Files which contribute to figures in the appendix. The 850 hPa winds are in "u850_winds" -- "jan01", "ph2", and "ph4" 
refer to which experiment they originate from (naming conventions as above) while "QE" and "QW" denote the imposed QBO states.

The folders RMM_qboclim and ROMI_qboclim are identical in data structure to the folders "RMM_ctrlclim" and "ROMI_ctrlclim" 
in the main body repository -- the difference is that tehse files were made using the "QBO climatology" as opposed to the 
"control climatology" as described in the appendix.
