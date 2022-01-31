# Time Series Analysis of NAICS: North American employment data from 1997 to 2019
![Naics](https://www.loc.gov/rr/business/images/naics.jpg) <br>

## I. Introduction
[NAICS](https://www.census.gov/naics/) (North American Industry Classification System) is an industry classification system developed by the statistical agencies of Canada ([Statistics Canada](https://www.statcan.gc.ca/eng/concepts/index)), Mexico ([Instituto Nacional de Estadistica y Geografia](http://www.inegi.org.mx/)), and the United States ([U.S. Economic Classification Policy Committee (ECPC)](https://www.census.gov/naics/?18967).

                Table 1: Structure of NAICS codes
|\# digits|   Industry level  |                        Example                            |
| :-:   |       -----       |                          ---                                |
|2    | Sector            | 23 : Construction                             |
|3    | Subsector         | 236 : Construction of buildings               |
|4    | Industry group    | 2361 : Residential building construction      |
|5    | Industry          | 23611 : Residential building construction     |
|6    | National industry | 236110 : Residential building construction    |

> ### I.1. Project goals
> This project aims to fill out the **Employment** column of an excel file of 15577 lines containing all the NAICS industry up to 4-digit from **Jan 1997** to **Dec 2018**. <br>
Additionally, we will  answer the following five questions:
> - How employment in Construction evolved over time and how this compares to the total employment across all industries?
> - When (Year)  was the employment rate the highest between the dedicated time frame?
> - Which industry sector, subsector or industry group has had the highest number of employees?
> - As a rapidly developping field, if Data Science industry level (Number of digits) in NAICS, is less or equal to 4 then how has Data Science employment evolved over time? Otherwise, What is the lowest industry level above Data Science and how did it evolve from 1997 to 2019? 
> - Are there industry sectorsn subsectors or industry groups for which the employment rate decreased over time?


### I.2. The data
To oustandingly address the above questions, we are provided with **15 csv files** (**5** files per level of aggregation) beginning with RTRA([Real Time Remote Access](https://www.statcan.gc.ca/en/microdata/rtra)) containing employment data by industry at different levels of aggregation; **2-digit NAICS, 3-digit NAICS**, and **4-digit** on one side. <br> 
Each of these files has the following columns in the same order from left to right:
-  SYEAR: Survey Year
- SMTH: Survey Month
- NAICS: Industry name and associated NAICS code in the bracket
- \_EMPLOYMENT\_: Employment 

On the other side there is an excel file **LMO_Detailed_Industries_by_NAICS.xlsx** that maps all the NAICS codes with the name of the corresponding industry.

#### Coming Next: Dashboard (with [Dash](https://dash.plotly.com/) for visualisations...
