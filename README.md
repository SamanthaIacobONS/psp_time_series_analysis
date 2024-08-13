# Public Sector Productivity Time Series Analysis

**Last Updated** : 13/Aug/2024

**Contributors**: Richard Marshall (<richard.marshall@ons.gov.uk>) and Samantha Iacob (<samantha.iacob@ons.gov.uk>)

## About 

This is a small project aimed at assessing the methods used by the Time Series Analysis Team for Nowcasting public sector productivity data from quality-adjusted annual data with a two year lag, and annualized quarterly data with a four month lag.
The PSP productivity nowcasts (up until 2019 for the purpose of analysing the models) are generated from this data using an R script and are stored in the *data/nowcast* subdirectory of this repository.

The notebook in this repo produces ADF and Ljung-Box Test statistics used to analyse the stationarity and autocorrelation of the residuals of the models used in Nowcasting (along with some plots which might be useful). The statistics are ouput to .xlsx files in the *output* subdirectory along with autogenerated summaries saved in .txt format. These have already been included in this repo using the Nowcast data provided to us but if you want to input different data then this could be useful.

This project was carried out as part of the [ONS DGO Data Apprenticeship Scheme](https://onsdigital.blog.gov.uk/2023/05/16/data-apprenticeships-at-the-office-for-national-statistics/) with thanks to Michaela Lawrence and Mark Hogan for their support.

## Instructions

Clone or save this repository to your computer and open *psp_analysis_by_model.ipynb* in Jupyter Notebooks.

Run the cells in order. Note that **cell 3** contains a *target* variable - this can be set to inputs, outputs or prods. This was done to improve the readability of the plotting sections of the notebook and also to make it easier to divide analysis work among multiple users. 

If you are missing libraries check *requirements_conda.txt* for details.

## Known Issues

The *data_importer* function in cell 4 is based on the file names currently generated from the Nowcast R script. Future versions of this script may create files with different version names so this cell will need to be updated in that case.

## Licence

Licenced under under the [Open Government Licence v.3.0](https://www.nationalarchives.gov.uk/doc/open-government-licence/version/3/).
