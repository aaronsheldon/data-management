---
layout: page
element: notes
title: Data entry
language: Excel
---

### Where to enter data

* Spreadsheet
* Text file
* Database
* Form (web or GUI databases)

* All of these are reasonable options
* When used properly spreadsheets or forms for databases can provide additional
protection against bad data being entered
* Be careful of data conversion issues from spreadsheets

> Show posts/papers on dates and gene names
> * https://genomebiology.biomedcentral.com/articles/10.1186/s13059-016-1044-7
> * https://datapub.cdlib.org/2014/04/10/abandon-all-hope-ye-who-enter-dates-in-excel/

### Tips from the trenches (@pxxpih)

From [here](https://twitter.com/pxxpih/status/819592744741937153)

- place metadata on a separate sheet within the workbook. Describe other sheets, columns, allowed values, units, guidelines.
- make data as columnar as possible. Instead of columns for each year, one column describing the year, with many rows. One way to check this -- do any column headings contain data?
- always have a physical interpretation for a single row. Is it one patient? One visit? A single observation at one site?
- don't version control using workbooks, sheets or columns. Use a version control system like git or svn.
- keep data type consistent within a single column, particularly do not introduce strings to a numeric column.
- for standardized codes have a sheet of reference values, this will aid in importing into a relational database, and with error checks.
- For excel, triple check date formatting. ISO numeric, either YYYY-MM-DD or YYYYMMDD, is recommended as it sorts correctly.
- If an entity (e.g. a site or quadrat) is represented across multiple rows, periodically re-sort by the entity and check to ensure values are conserved. For example, if there are multiple visits per patient, make sure there is no drift in birth dates, self identified gender, etc.
- If you notice the same column structure across multiple sheets, compile into a single sheet with an new column containing an appropriate indicator of the source. Your future self will thank you.
- When logging data onto paper first (field work, patient charts etc.) lay out the paper forms with the aim to speed transcription. In general this means ordering paper forms and spreadsheet columns from most general to most specified. This will allow you, on paper and digitally, to "ditto" repeated identifiers. 
- Keep a separate log sheet for exceptions (notes really). Remember that you won't remember what your various coded hints meant.
- Indicate a failure to classify as such. These are your most important observations! They allow you to calibrate observation error. You can then report of N observations k could not be classified. You can then report your observation error based on the hypothetical assignment of the k to the various categories.
- When capturing interval data, particularly time, decide ahead of time, and document, your choice of boundary inclusions (open versus closed topology). As the choice of whether the start and end boundaries are inclusive has important implications for the calculation of durations. For example, in working with daily data it is typical for the start and end dates to be inclusive so that `duration = end - start + 1`. This concern generalizes to all forms of rounding and significant digits.
- For each column determine and document the interpretation of nulls, or empty cells. Does it mean not observed? Indefinitely in the future? Indefinitely in the past? Some coding conventions involve specifying a code for the reason for missing. This is rarely of use. Statistical techiniques, such as survival analysis, that can incorporate incomplete or censored data generally are only concerned with absence or presence.
- Record the temporal and spatial bounds of a set of observations, such as the beginning and end of a data capture period. This is important for working with statistical techniques that incorporate missing, and censored data. The temporal and spatial bounds place censoring limits on the possible values of the data. Or in the worst case can be used as uninformative uniformly distributed priors.

### Quality Assurance

* Stopping bad data from ever being entered
* Let's us set rules about what values can be entered into a column

* Select an area of cells, most often a column
* `Data -> Data Validation`
* Choose the data type: `Whole numbers` (only that type can be entered)
* Set limitations
    * Use `Data` to set the type of limitation: `between` 
    * Then use additional boxes to provide specifics: `1` and `10`
* Add a message to explain what goes in a cell in `Input Message`
* Add a useful error message using `Error Alert

* Make lists of choices
    * `Allow` = `List`
    * Enter list values in `Sources`: DM, DO, DS, PP, PM

> Demo a data entry form in Access or Google Forms

### Quality Control

* Looking for bad data that has already been entered
* Sort
* Graph
* Check for realistic ranges of values
