# Best Practices in Tabular Data

Much of the Region’s data is contained in spreadsheets \(i.e., tabular data, most commonly MS Excel files\). Multiple spreadsheets within the same file can contain data and derivatives of the data \(tables, summaries, pivot tables, formulas, figures\). There are some best practices to use when dealing with this type of data. Examples of untidy vs tidy datasets are given in [Appendix C](../../appendix-c-example-of-untidy-vs.-tidy-tabular-data.md).

* One sheet in the file should contain only a clean version of the data. Nothing else should be on this sheet. This is sometimes referred to as tidy data. In tidy data:
  * The first row contains variable names, each column represents one variable. Variable names should use only letters, numbers, dashes, “-“, and underscores, “\_”. Do not use spaces or any other characters. The variable name should include the unit where this is relevant \(e.g., length\_cm and weight\_gm\).
  * Each row after the first row should represent one observation.
  * Avoid formatting information in this sheet \(e.g., comma in the thousands place, font settings, border lines, colors, etc\). If the formatting is there to convey some information, consider adding a new variable to record that information instead.
  * For the purposes of tidy data, blank cells indicate that the data point is missing. “0” in a cell means that the data point was collected and it was “0”. Deviations from this convention should be recorded in the data dictionary \(see below\).
  * The tidy data sheet, in addition to being part of the workbook, should also be saved in an open format \(e.g. Text  or CSV\) using the same name as the Excel file \(e.g., fish\_data.xlsx and fish\_data.txt\) in the same archive folder as the Excel file.
* One sheet in the file should provide a brief description of each variable in the tidy data. Each row of this sheet represents one variable. This is termed the data dictionary and will be part of the metadata record for the tidy data. An example and a template for the data dictionary is available [here](https://drive.google.com/open?id=17p0hwSsKFoDryC5EDGPkxChBjKWvN0V-2U-6SAO3NKQ). 
* Other sheets in the file can contain summaries of the data \(pivot tables\), graphical representations of the data \(figures\), or derived quantities from the data \(formulae, macros, etc\). Avoid including metadata on these sheets.
* One sheet in the file should provide a brief description of each sheet in the file \(what does it contain, any relevant information about its use\). Each row of this sheet represents one sheet of the file. First column is the sheet name, the second column is the sheet description.
* Save the original workbook in the most recent format supported by the application. For example, save Excel files in .xlsx format rather than .xls format.

