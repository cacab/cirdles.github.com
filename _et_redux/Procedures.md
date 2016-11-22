---
layout: project-page
help: et_redux
title: Procedures
category: Help
reference: Procedures
---

New Project from Raw Data

1. Open ET_Redux - note that this will generate two html files, ChangeLog.html and Credits.html
2. To start, click "Project" in the top left corner.
3. Then click "New Project" from Raw Data.
4. Click "LA-ICP-MS".  Note that IDTIMS raw data is currently processed by our software [Tripoli](http://cirdles.org/projects/tripoli/).
5. Now you will see the Project Manager interface where you specify your project. Start by entering your Project Name and then choosing the appropriate:
  * File Handling Protocol
  * Raw Data Template
  * Analysis Purpose
6. Finally, click "Prepare to load/Process Raw Data." Then, depending on your file handling protocol you will be able to select your data file or data folder and then click "Open" to show the parameters manager. If you use folders, be sure that all necessary files are present.
7. Confirm that all parameters are correct - the defaults are shown initially.
8. Full Uncertainty propagation is the default - use the fast option to explore datasets only.
9. Select your Primary Reference Material.  Note the default is set in the Lab Settings Manager.
10. Now you are ready to start the reduction process. You can either start a live session while the mass spectrometer is producing data or proceed to reduce an already-collected dataset as explained below.

Live Data Reduction Processing:

1. Click "Save and Monitor/Process Raw Data"
2. Once the live data monitor is launched you will have to wait for at least 3-4 analysis to be recorded by the mass spectrometer software and processed by ET_Redux before seeing any data.
3. To reject an analysis, right click on the selected fraction name in the report table located in the bottom portion of the manager and it will be sent to the rejected fractions tab but will still be reduced.
4. To look at individual samples (Reference Materials or Unknowns), double click on the project name in the panel to the left of the concordia, and a drop down menu will show all available groups to view on Concordia and on the PDF.  Note that the reference materials both primary and secondary will not appear in the PDF view.
5. To set filters for percent discordance and percent uncertainty, adjust the sliders in the panel under the PDF. To apply them to the Concordia plot, select "apply filters" checkbox under the Concordia.  To set the sliders to the default values specified in the lab data manager, click "Default", and to clear the filters, click "Clear".
6. To change what dates are shown on the PDF, select one of the three dates (6/8, 6/7, or best date). We suggest the best date option.
7. Best date filter can be changed while you are looking at unknowns in Concordia space by sliding the blue best date handle on the vertical axis.
8. When a fraction is removed be patient as it will take until the next primary reference material fraction to update the session.
9. If you need to refresh, click "Refresh Views"
10. Wait until the run has completed and proceed to Project Raw Data Manager (see below).

Project Raw Data Manager

1. Consider using the following view options singly or in combination to explore your data:
  * Y-axis Scaling set to Independent
  * Show All Local Y-axis
  * Make horizonal zoom very tight to highlight patterns in data
2. Start with the default "Intercept" method tab.
3. Review the reference materials to make sure ratios are within acceptable rages. It will be very clear when an analysis is bad. You will either see a very large scatter in data points or the fit line will be far off the data points.  Be sure to select the appropriate fit functions on a ratio-by-ratio basis, or even for each graph.
4. Click "Show Session" button.
5. The time-based session views for each ratio plot the reference materials and their 1-sigma absolute uncertainties in black and over-dispersion of uncertainties in red, if calculated. Each session can be fitted with a choice of mean, line, exponential or spline functions. 
6. To remove a data point for a reference material, hover over the black dot and right click. You will be asked to “exclude this fraction", click on it and the black dot will change to red indicating it has been removed.
7. Once you have removed all unwanted data points you MUST click "Refit" on the left update the plot and MSWD. 
8. Next, click "Fit Unknowns" and evaluate each fraction and ratio for the unknowns and the secondary reference materials, which are also treated as unkowns.
9. When you are happy with your fits, to complete your reduction click "Update Report Table", which will remain grayed out until it finishes and then returns to the color white.
10. Return to the main window showing the data table and click "Sample Dates" in the bottom right to launch the sample date manager with the concordia, weighted means, and PDF plots and views.
	
New Sample Analysis for ID-TIMS

1. At the main menu, click "Sample" and then click "New Sample Analysis for ID-TIMS" to launch the ID-TIMS Workflow Manager for ANALYSIS MODE of a Sample.  You can always return to this window by clicking the "Manage Sample" menu item under the main emanu "Sample".
2. Provide the "Local Sample Name" and "IGSN".  SESAR is the default registry to date.
3. Select the "Analysis Purpose" and  the "Phsyical Constants Model".
4. For each aliquot, provide the name and then click "Add Name" to add the aliquot to the left-hand list.  Once this list is populated with the names of the aliquots, clicking each name sets up the next step of either manually "inserting fractions" or "importing a folder of fractions", which consists of XML files produced by Tripoli or similar software.  These XML files must conform to the schema found [here](https://raw.githubusercontent.com/EARTHTIME/Schema/master/UPbReduxInputXMLSchema.xsd).
5. Fractions and aliquots may be removed using the appropriate buttons.  If importing is done, the default fraction should be removed.
6. For each fraction of each aliquot complete the entries in the interactive data table at the bottom of the window.
7. For manual update, Click "Close and Save" button.
8. For Live Workflow, be sure to set the following parameters before clicking "Close and Save" button.
  * one
  * two
  * three