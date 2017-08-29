



<br>

[![Downloads](http://cranlogs.r-pkg.org/badges/grand-total/Rilostat)](https://cran.r-project.org/package=Rilostat) 
 [![Downloads](http://cranlogs.r-pkg.org/badges/iostat)](https://cran.r-project.org/package=Rilostat) 
 [![Coverage Status](https://img.shields.io/codecov/c/github/ilostat/Rilostat/master.svg)](https://codecov.io/github/ilostat/Rilostat?branch=master) 

<!-- [![AppVeyor Build Status](https://ci.appveyor.com/api/projects/status/github/ilostat/Rilostat?branch=master&svg=true)](https://ci.appveyor.com/project/ilostat/Rilostat) -->
<!-- [![CRAN_Status_Badge](http://www.r-pkg.org/badges/version/Rilostat)](https://cran.r-project.org/package=Rilostat) -->

<br>

## ilostat R package

<!-- README.md is generated from README.Rmd. Please edit that file -->


The [ILO](https://www.ilo.org)'s main online database, [ILOSTAT](https://www.ilo.org/ilostat), maintained by the [Department of Statistics](https://www.ilo.org/stats), 
is the world's largest repository of labour market statistics. It covers all countries and regions and a wide range of labour-related topics, including employment, unemployment, 
wages, working time and labour productivity, to name a few. It includes time series going back as far as 1938; annual, quarterly and monthly labour statistics; country-level, 
regional and global estimates; and even projections of the main labour market indicators.
  
ILOSTAT's website provides immediate access to all its data and related metadata through different ways. Basic users can simply view the desired data online or download it in Excel or csv formats. 
More advanced users can take advantage of ILOSTAT's well-structured [bulk download facility](http://www.ilo.org/ilostat/faces/oracle/webcenter/portalapp/pagehierarchy/Page30.jspx) ([user guide](http://www.ilo.org/ilostat-files/WEB_bulk_download/ILOSTAT_BulkDownload_Guidelines.pdf)), or the SDMX web service ([user guide](http://www.ilo.org/ilostat/content/conn/ILOSTATContentServer/path/Contribution%20Folders/statistics/web_pages/static_pages/technical_page/ilostat_appl/SDMX_User_Guide.pdf)).

  
The ilostat R package (`'Rilostat'`) was designed to give data users the ability to access the ILOSTAT database, search for data, rearrange the information as needed, download it in the desired format, and 
make various data visualizations, all in a programmatic and replicable manner, with the possibility of quickly re-running the queries as required.

#### Main features of the ilostat R package 

- Provides access to all annual, quarterly, and monthly data available via the ILOSTAT [bulk download facility](http://www.ilo.org/ilostat/faces/oracle/webcenter/portalapp/pagehierarchy/Page30.jspx) ([user guide](http://www.ilo.org/ilostat-files/WEB_bulk_download/ILOSTAT_BulkDownload_Guidelines.pdf))
- Allows to search for and download data and related metadata in English, French and Spanish
- Gives the ability to return `POSIXct` dates for easy integration into plotting and time-series analysis techniques
- Returns data in long format for direct integration with packages like `ggplot2` and `dplyr`
- Gives immediate access to the most recent updates
- Allows for `grep`-style searching for data descriptions and names
- Provides access to the ILOSTAT catalogue of related descriptive metadata ([user guide](http://www.ilo.org/ilostat/content/conn/ILOSTATContentServer/path/Contribution%20Folders/statistics/web_pages/static_pages/technical_page/ilostat_appl/SDMX_User_Guide.pdf))

#### Acknowledgements

The developer of this package drew extensive inspiration from the [eurostat R package](https://cran.r-project.org/web/packages/eurostat/) and its related documentation:  
  - [Retrieval and Analysis of Eurostat Open Data with the eurostat Package](https://journal.r-project.org/archive/2017/RJ-2017-019/RJ-2017-019.pdf) - [Leo Lahti](https://github.com/antagomir), [Przemyslaw Biecek](https://github.com/pbiecek), [Markus Kainu](https://github.com/muuankarski) and [Janne Huovari](https://github.com/jhuovari). R Journal 9(1), 385-392, 2017.

## <a name="installation"></a>Installation



```r
install.packages("Rilostat")
```


To install the development version, use the following command:


```r
if(!require(devtools)){install.packages('devtools')}
install_github("ilostat/Rilostat")
```

The ilostat R package (`'Rilostat'`) includes the following functions:


```r
require(ilostat)
as.data.frame(ls("package:Rilostat"))

```



We do not expect to update the ilostat R package too often, but based on questions and remarks from ILOSTAT 
data users, we will progressively create more examples, 
tutorials, demos and apps. We will publicly share all of this via the function:


```r
ilostat()

ilostat('GettingStarted')
```


### Contribute

Contributions are very welcome:

  * [Use issue tracker](https://github.com/ilostat/Rilostat/issues) for feedback and bug reports.
  
  * [Star us on the Github page](https://github.com/ilostat/Rilostat)
  
### Permission to reproduce ILO publication and data

The reproduction of ILO material is generally authorized for non-commercial purposes and within established limits. 
However, you may need to submit a formal request in certain circumstances. for more information please consult:

http://www.ilo.org/global/copyright 

http://www.ilo.org/global/copyright/request-for-permission
