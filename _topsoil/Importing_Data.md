---
layout: project-page
help: topsoil
title: How to Import Data
category: Help
reference: importing
---
When importing your data into Topsoil, you have a few options. The most important thing to remember is the way that Topsoil organizes its data. The data must be in five columns, with each column representing X axis values, Y axis values, X uncertainty values, Y uncertainty values, and rho (correlation coefficient) values, in that order. For example, for a Uranium-Lead analysis, data may be arranged like this:

<img src="/assets/images/headers-emptyTable.png" width="100%">

Whenever you import data, a helper will appear where you will be able to pick which of your data columns correspond to the layout above.

In each tab, there is a set of labels denoting the proper organization of data. Beneath those labels are the column names, which Topsoil will try to determine based on what you provide it. If Topsoil detects one or more rows that do not consist of numerical values, it will use those as the column names. Up to two header rows will be read; the rest will be ignored.

<font size="4"><b>Importing from a File – (.csv, .tsv, .txt):</b></font>

1. Navigate to Table >> Import Data Table. Select “From File”.
  <img src="/assets/images/import-from-file.png" width="100%">

2. A file chooser will appear that will allow you to select the proper file from your computer.
  <img src="/assets/images/open-table-file.png" width="100%">

3. (If the delimiter request window doesn't appear, skip to 4.) If you are importing a .txt file, and Topsoil can’t automatically determine how your data values are separated, you’ll be presented with a dialog box. You can select from common data separators from the drop-down list, or, by selecting “Other”, you can specify your own. Once you've specified a separator to use, click "OK".
  <img src="/assets/images/delimiter-request.png" width="100%">

4. A helper window will appear containing a preview of your data. The column names and first five data rows are shown as they would be imported into Topsoil. Above that is a row of drop-down lists with the names of each of the five plotting variables that Topsoil uses. From this screen, you’re able to use the drop-down lists to select which of your data columns correspond to the which variables. By default, the first five will be selected. Important: Any columns that aren’t selected will NOT be imported into Topsoil, and that any variables that don’t have columns assigned to them will be filled with 0.0s. Support for extra columns will be added in the future.
  <img src="/assets/images/import-helper.png" width="100%">

5. In the same window, there is a drop-down list towards the bottom for selecting the format of your uncertainty values. The values will be in the table and editable as the format you specify, but Topsoil will convert them into 1-sigma absolute format so that you can apply different formats to a plot. Select one and click "Finish".

6.	You’re done! Topsoil will populate the table with the provided values. Please note that the default [isotope system](#is_sys) is Generic, which will not support any special plotting features provided for each type of isotope system. The isotope system can be changed freely from a drop-down list in the Plot Manger section, beneath the table.  
  <img src="/assets/images/plot-manager.png" width="100%">


<font size="4"><b>Importing from the Clipboard:</b></font>

1. Navigate to Table >> Import Data Table. Select “From Clipboard”.
  <img src="/assets/images/import-from-clipboard.png" width="100%">

2. (If the delimiter request window doesn't appear, skip to 3.)If you are importing a .txt file, and Topsoil can’t automatically determine how your data values are separated, you’ll be presented with a dialog box. You can select from common data separators from the drop-down list, or, by selecting “Other”, you can specify your own. Once you've specified a separator to use, click "OK".
  <img src="/assets/images/delimiter-request.png" width="100%">

3. A helper window will appear containing a preview of your data. The column names and first five data rows are shown as they would be imported into Topsoil. Above that is a row of drop-down lists with the names of each of the five plotting variables that Topsoil uses. From this screen, you’re able to use the drop-down lists to select which of your data columns correspond to the which variables. By default, the first five will be selected. Important: Any columns that aren’t selected will NOT be imported into Topsoil, and that any variables that don’t have columns assigned to them will be filled with 0.0s. Support for extra columns will be added in the future.
  <img src="/assets/images/import-helper.png" width="100%">

4. In the same window, there is a drop-down list towards the bottom for selecting the format of your uncertainty values. The values will be in the table and editable as the format you specify, but Topsoil will convert them into 1-sigma absolute format so that you can apply different formats to a plot. Select one and click "Finish".

5. You’re done! Topsoil will populate the table with the provided values. Please note that the default [isotope system](#is_sys) is Generic, which will not support any special plotting features provided for each type of isotope system. The isotope system can be changed freely from a drop-down list in the Plot Manger section, beneath the table.
  <img src="/assets/images/plot-manager.png" width="100%">
