# UECombined
A combined HUX and ISB model, which includes the scapula.

It´s complete project description in the sense of the Nimue platform (http://nimue-platform.motion-science.org) which includes the model definition, plot sheet configuration etc. It can be used by the Upperlimb software (http://upperlimb.orat.de/doku.php). 

-----------------
== Upperlimb 0.928 - 2019-01 ==
------------------------

**Added**
   * PlotSheet declaration files for none, first, second or both static positions (as a WORKAROUND for the Plotsheet Bug which results in broken selection/navigation for uncomplete data); [[kinematic_model&#sheetdefs | here]]

**Changed**
   * Upperlimb models upgraded to Version 1.7 (Determination of scapular rotation for static positions  in projection angles). The new angles are shown per default in the plot sheets.
   * Update to [[http://nimue-platform.motion-science.org/doku.php?id=start&#changelog | Nimue Platform 0.92 - 2018-11]]

**Planed/known bugs**
   * If not data is availble to be plot in a plot sheet, the selection/navigation shows strange behavoir (select/deselct does not work ...)
   * In rare cases an additional wrong RElePhase, whichs ends at the end of the trial, is added, e.g. RSA3D-317, Trial 12
   * The action "Process..." tries to access directly FilterNodes instead usage of the indirection of the Lookup. This can fail.
   * Automatically deleting output files, if process is canceled
   * Planed to fix in this version: Static shoulder angles measurements over 90 degree sometimes show offset about 180 degree.
   * The resizing behavoir of the window showing processed data is unhandy. If the status switched from processed data not available to available the size should be grown vertically automatically to show the new processed data node.
   * Extention of the model with R/LSHRCardanISB based on Thorax- and Humerus coordinate systems following the ISB recommendations exactly.
