# MATPLOTLIB Visualizations

See the jupyter notebook `Sivasangaran V Matplotlib Visualizations.ipynb` for code and plots.

# Bar plot and Box Plot

These plots have been constructed using the National Family Health Survey dataset, 2019-2021[1].

The National Family Health Survey (NFHS) is a large-scale, multi-round survey conducted in a representative sample of households throughout India. The NFHS is a collaborative project of the International Institute for Population Sciences(IIPS), Mumbai, India; ICF, Calverton, Maryland, USA and the East-West Center, Honolulu, Hawaii, USA. The Ministry of Health and Family Welfare (MOHFW), Government of India, designated IIPS as the nodal agency, responsible for providing coordination and technical guidance for the NFHS. NFHS was funded by the United States Agency for International Development (USAID) with supplementary support from United Nations Children's Fund (UNICEF). IIPS collaborated with a number of Field Organizations (FO) for survey implementation. Each FO was responsible for conducting survey activities in one or more states covered by the NFHS. Technical assistance for the NFHS was provided by ICF and the East-West Center. [2]

## References:

1. https://data.gov.in/resource/india-districts-factsheets-national-family-health-survey-nfhs-5-2019-2021
2. http://rchiips.org/nfhs/about.shtml

# Bar Plot

**Fig.1** % of female population who attended school (6 years and above) in Karnataka

# Conclusion

In Bangalore, the most no. of females attended school, while in Yadgir, the least no. of females attended school.

# Box Plot

**Fig. 2** Sex Ratio distribution throughout India
1. Sex ratio at birth for children born in the last five years (females per 1,000 males)
2. Sex ratio of the total population (females per 1,000 males)

We can observe that the sex ratio is also taking negative values.

![image.png](attachment:image.png)

From this figure, we can see that the negative values are actually written in the excel sheet within brackets. According to [1], if the written values are within brackets (), then it means that the ratio or percentage or average was computed using between 25 to 49 sample values. What this means in this figure is that in the districts, which have negative (or bracketed) sex ratio values, the population of men examined or surveyed is between 25 to 50, which essentially means that this value is not a true representative of the population being observed. 

In the excel sheet, we can observe that in Bhopal, only 38 males were surveyed (15-54 years), which indeed matches with this observation. 

To handle this situation, we can remove the values within parentheses (the negative values) using `df.drop()` function or we can keep those values, taking the absolute value. I have retained those values, by taking absolute values.

So, in figure in the website, the box plot is the corrected version, after doing this "data preprocessing".

## References:
1. https://www.dhsprogram.com/pubs/pdf/DM56/DM56.pdf

# Conclusion

We can observe that the sex ratio of the new born children is less than that of the total population. This means, sex ratio is likely to decrease in the future. Also, there are still households, which prefer having male children compared to female children.

# Scatter Plot

The dataset used for this plot is the Consumer Price Index dataset. [1]

Consumer Price Index (CPI) measures changes over time in the general level of prices of goods and services that households acquire for the purpose of consumption. For the construction of CPI numbers, two requisite components are weighing diagrams (consumption patterns) and price data collected at regular intervals. The data refers to the All India Consumer Price Index with the base year 2012 equal 100 and combined for both rural and urban areas. All India Consumer Price Index (CPI) - Cereals and products have increased from 144.9 in January 2021 to 148.2 in November 2021 showing an increase of 3.3 points. All India Consumer Price Index (CPI) - Vegetables has increased from 194.2 in January 2021 to 199.2 in November 2021showing an increase of 5 points. All India Consumer Price Index (CPI) - Fruits has increased from 149.6 in January 2021 to 156.5 in November 2021 showing an increase of 6.9 points. All India Consumer Price Index (CPI) - General index has increased from 157.3 in January 2021 to 166.7 in November 2021 showing an increase of 9.4 points. Consumer Price Index (CPI) for the rural area, the General index has increased from 158.5 in January 2021 to 167.6 in November 2021 showing an increase of 9.1 points. Consumer Price Index (CPI) for the urban area, General index has increased from 156 in January 2021 to 165.6 in November 2021 showing an increase of 9.6 points. [2]

## References:

1. https://data.gov.in/resource/all-india-consumer-price-index-ruralurban-upto-november-2021
2. https://visualize.data.gov.in/?inst=a5df75bc-4578-48ad-bc9d-e6eb4b63de0a&vid=106532

### Note that I have plotted only from Jan 2013 to Apr 2016 for simplicity

# Conclusion

We can observe that there is an increasing trend in the price of all the commodities. However, the prices of vegetables exhibits large fluctuations.