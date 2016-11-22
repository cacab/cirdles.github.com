---
title: Using the Workflow Manager
reference: using-workflow-manager
---

The Workflow Manager can be accessed by clicking *Sample* in the top menu of ET_Redux. You will be presented with several options for creating and editing a sample. To create a new sample, click *New Sample Analysis for ID-TIMS*. This opens the Workflow Manager for a new sample.

**Editing the Sample Name**

To change the name of your sample input the desired name into the *Local Sample Name* box.

**Adding an IGSN ID**

To specify the IGSN, select the registry from the *Registry* drop down menu and input the ID into the *Sample ID* box. Click the button to the right of where you input the ID to validate the registry.

**Adding Aliquots**

To add an aliquot to your sample, type the name of the aliquot in the *Aliquot Name* box and click *Add Name*. This will add your aliquot to your sample's aliquot list. You can select an aliquot from that list to edit or remove it. If you ever want to change the name of an aliquot, select it from the list, change the name in the Add Name box, and click Save Edited.

**Adding Fractions with Live Workflow**
The Live Workflow mode establishes a direct link between Tripoli and ET_Redux. To enable Live Workflow, you must create a folder called "SampleMetaData" and then click the *Set SampleMetaData Folder* button. Tripoli must also be told the location of this SampleMetaData folder.  In Tripoli, point to this SampleMetaData folder with the *Set Live Workflow Data Folder* item from the Control Panel menu. Clicking the *START Live Workflow* button at the bottom of ET_Redux’s main screen immediately imports data from Tripoli and prompts ET_Redux to update its calculations. 


**Adding Fractions Manually**
Select an aliquot from the sample's aliquot list. Then click *Import Fraction Files* and navigate to your sample's fraction files which are saved as XML documents. You can import multiple fractions at a time by holding CTRL and clicking the files.




