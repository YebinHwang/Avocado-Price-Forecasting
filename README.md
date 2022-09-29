# Avocado-Price-Forecasting

Tableau Visualization: https://public.tableau.com/app/profile/yebin.hwang?authMode=activationSuccess

Kaggle Dataset & Description: https://www.kaggle.com/datasets/timmate/avocado-prices-2020?resource=download

### About Dataset
UPD
Updated on Feb 26, 2021 with the latest HAB data for 2020 (up to 2020-11-29). Newer data, incl. for 2021, have not yet been published by the HAB.

Context
This is an updated version of the avocado dataset originally compiled from the Hass Avocado Board (or HAB, for short) data and published on Kaggle by Justin Kiggins in 2018. The dataset features historical data on avocado prices and sales volume in multiple cities, states, and regions of the USA.

Content
This updated version contains data from 4 January 2015 up to 17 May 2020, whereas the original dataset uploaded by Justin provides data only for the time span from 2015 to the beginning of 2018. The updated dataset was created by downloading the data for years 2018 to 2020 from the Hass Avocado Board website in August 2020, preprocessing it and merging it with Justin's dataset.

The new data was downloaded from this page of the HAB's website which allows downloading the data for years 2017 -- 2020 (as of August 2020). To download some new data, scroll down to the bottom of the section "Totals by PLU" and click the "Download 20XX Weekly Retail Volume & Price Report" button (the "XX" are the two last digits of the year you are downloading the data for).

Notebooks for creating and updating this dataset
This dataset was created using this Colab notebook. If you want to add even more fresh data to this dataset, you can download the new data from the HAB's website and add it to this dataset using this Colab notebook.

Difference from the original dataset
Please note that, besides containing more data, this dataset differs from the original one in the following points:

All column names were converted to "snake_case" for more consistency in naming and to provide access to column values using a period, e.g., df.average_price.

The column region was renamed to geography (as it is called in the HAB's data) to avoid the confusion between actual regions (e.g., West, Midsouth, etc.), cities (e.g., San Francisco, Atlanta, etc.), states (e.g., California, South Carolina, etc.), and other geographical names of the US.

For the data to be merged, the geographical names in the region column of the original dataset had to match the corresponding geographical names of the new HAB's data. For the sake of readability and clarity, the original HAB's naming style of geographical names was chosen. For that reason, some of the geographical names in the region column of the original dataset were renamed, for instance, BaltimoreWashington was renamed to Baltimore/Washington, DallasFtWorth was renamed to Dallas/Ft. Worth, TotalUS was renamed to Total U.S., and so on.

The data is already sorted by date and geographical names.

Description of columns
Please refer to the main page of the original dataset.

A note on the data
Please note that, according to this page, the Total U.S. data is somewhat aggregated for the following 8 geographical areas of the US: California, Great Lakes, Midsouth, Northeast, Plains, Southeast, South Central, and West. However, averaging data for these regions and areas does not result in the entries equal to those of the Total U.S. data, so be careful with that.

Acknowledgements
Huge thanks to Justin Kiggins for the original dataset and to Hass Avocado Board for making the data publicly available!
