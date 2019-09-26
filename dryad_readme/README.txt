This README.txt file was generated on 20190926 by Jon Minton

-------------------
GENERAL INFORMATION
-------------------

Title of Dataset: Data from: Recent adverse mortality trends in Scotland: comparison with other high-income countries

Author Information (Name, Institution, Address, Email)

	Principal Investigator: Lynda Fenton, NHS Ayrshire & Arran. lynda.fenton@nhs.net 
	Associate or Co-investigator: Jon Minton, NHS Health Scotland. jon.minton@nhs.net
	Associate or Co-investigator: Julie Ramsay, National Records of Scotland. Julie.Ramsay@nrscotland.gov.uk
	Associate or Co-investigator: Maria Kaye-Bardgett, National Records of Scotland. maria.kaye-bardgett@nrscotland.gov.uk
	Associate or Co-investigator: Colin Fischbacher, NHS National Services Scotland. colin.fischbacher@nhs.net
	Associate or Co-investigator: Grant Wyper, NHS Health Scotland. gwyper@nhs.net
	Associate or Co-investigator: Gerry McCartney, NHS Health Scotland. gmccartney@nhs.net
	Alternate Contact(s): http://www.healthscotland.scot/contact-us/general-enquiries/your-general-enquiry

Date of data collection (single date, range, approximate date): 2018-2019

Geographic location of data collection: Glasgow, Scotland

Information about funding sources or sponsorship that supported the collection of the data:

The data were collated mainly by the Human Mortality Database, and collected from a range of international bodies, including the NRS.
All researchers are salaried employees of the NHS or NRS and received no specific external funding for this work. 

Information about IRB or ethics committee that approved the research: 
This research did not involve research on human individuals and did not require specific ethics approval.

--------------------------
SHARING/ACCESS INFORMATION
-------------------------- 

Licenses/restrictions placed on the data, or limitations of reuse: 
CC0 1.0 Universal (CC0 1.0)

Recommended citation for the data:
Fenton L, Minton J, Ramsay J, Kaye-Bardgett M, Fischbacher C, Wyper G, McCartney G (2019) Data from: Recent adverse mortality trends in Scotland: comparison with other high-income countries. Dryad. Dataset. https://doi.org/10.5061/dryad.hc627cj

Citation for and links to publications that cite or use the data:
Fenton L, Minton J, Ramsay J, Kaye-Bardgett M, Fischbacher C, Wyper G, McCartney G (2019) Recent adverse mortality trends in Scotland: comparison with other high-income countries. BMJ Open.

Links to other publicly accessible locations of the data:

Human Mortality Database (HMD): https://www.mortality.org/
NRS: https://www.nrscotland.gov.uk/statistics-and-data/statistics/statistics-by-theme/vital-events/deaths/deaths-background-information/quality-of-nrs-data-on-deaths
ONS: https://www.ons.gov.uk/peoplepopulationandcommunity/birthsdeathsandmarriages/lifeexpectancies/datasets/nationallifetablesunitedkingdomreferencetables

Links/relationships to ancillary or related data sets: 

Data and RStudio project scripts in Github at https://github.com/JonMinton/Segmented-Regression


--------------------
DATA & FILE OVERVIEW
--------------------

File list (filenames, directory structure (for zipped files) and brief description of all data files):


HMD Scotland data time trend analysis.xlsx
 - excel workbook. Description as per title. Uses data from NRS and HMD.
Life expectancy international_updated Jan 2019 - inc. sensitivity analysis.xlsx
 - Excel workbook. Description as per title. Uses data mainly from ONS 
Segmented regression trend chart.xlsx
 - graphic showing results from segmented regression performed in R using (mainly) HMD data. R script included to produce analyses themselves.
Summary findings from segmented regression.xlsx
 - summary table of results from segmented regression performed in R using (mainly) HMD data. R script included to produce analyses themselves.

Relationship between files, if important for context:  
The majority of the submitted files summarise and present analyses performed in the following Rstudio project, available for download as a github repository at the following location:
https://github.com/JonMinton/Segmented-Regression.git

Additional related data collected that was not included in the current data package:
Some analysis scripts and derived data were produced in Stata before the use of R was adopted. Due to the size of some of these files, and the fact no results from this stage were included in the final submission, they have not been included in the data repository. 

If data was derived from another source, list source:
See links above

If there are there multiple versions of the dataset, list the file updated, when and why update was made:
Some of the scripts used to generate the results were modified after submission and acceptance. The only changes made were to the base location referred to in R markdown documents because these documents were moved to a separate directory to reduce file clutter. All scripts have been tested and generate the analyses reported. 


--------------------------
METHODOLOGICAL INFORMATION
--------------------------

Description of methods used for collection/generation of data: 
The HMD has a detailed methods protocol available here: 
https://www.mortality.org/Public/Docs/MethodsProtocol.pdf
The ONS and NRS also have similar methods for ensuring data consistency and quality assurance. 

Methods for processing the data: 
The segmented regression was conducted using the 'segmented' package in R. The recommended references to this package and its approach are here:
  Vito M. R. Muggeo (2003). Estimating regression models with unknown break-points. Statistics in Medicine, 22, 3055-3071.

  Vito M. R. Muggeo (2008). segmented: an R Package to Fit Regression Models with Broken-Line Relationships. R News, 8/1,
  20-25. URL https://cran.r-project.org/doc/Rnews/.

  Vito M. R. Muggeo (2016). Testing with a nuisance parameter present only under the alternative: a score-based approach with
  application to segmented modelling. J of Statistical Computation and Simulation, 86, 3059-3067.

  Vito M. R. Muggeo (2017). Interval estimation for the breakpoint in segmented regression: a smoothed score-based approach.
  Australian & New Zealand Journal of Statistics, 59, 311-322.

Software- or Instrument-specific information needed to interpret the data, including software and hardware version numbers:
The analyses were conducted in R version 3.6.1 and Microsoft Excel 2013

Standards and calibration information, if appropriate:
Not applicable

Environmental/experimental conditions:
Not applicable

Describe any quality-assurance procedures performed on the data:
Reproducible code and datasheets performed and checked by at least two authors.

People involved with sample collection, processing, analysis and/or submission:
See list of authors

--------------------------
DATA-SPECIFIC INFORMATION 
--------------------------

####################
HMD international_updated Jan 2019.xlsx
Comprises 20 worksheets, of which 14 contain data.
These data are arranged by country and by year.
Missing data codes: ""
The tab 'contents and sources' provides descriptions of the data source and contents of each sheet.

#####################
HMD Scotland time trend analysis.xlsx
Comprises 5 worksheets, including a combination of data and charts. 
The sheet 'contents' describes the data source and contents of other sheets.
The variables include year, life expectancy, and various measures of change in life expectancy
Missing data codes: ""

######################
Segmented regression chart.xlsx
Comprises 2 worksheets, 'Data' and 'Chart'.

Variables within the 'data' worksheet include:
Year
4 quarter rolling period ending
Female observed mortality rate
Female predicted by one-break model
Female predicted by two-break model
Male observed mortality rate
Male predicted by one-break model
Male predicted by two-break model
Chart breakpoint indicator
Missing data codes:  (blank space)



