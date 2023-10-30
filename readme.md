# P4-Job_satisfaction

## Description

The project is a comprehensive analysis of the factors affecting job satisfaction in various European countries, using data from Eurostat for the year 2018. It employs Python and a range of data visualization techniques to delve into the relationships between socio-economic indicators and job satisfaction.  

The project concentrates on key metrics such as weekly working hours, net income, the proportion of remote workers, and the prevalence of weekend work. The primary objective is to uncover how these variables influence job satisfaction and whether there are variations among different European countries.  

The analysis employs barplots to compare indicators across countries, scatter plots to explore relationships between multiple indicators for each country, map visuals to visualize geographical variations, and a regression decision tree to model the influence and importance of different indicators on job satisfaction.  

This multifaceted approach will provide valuable insights for understanding job satisfaction dynamics in a European context.


### Variable analysis.  

The series of graphs provide a comparative analysis of multiple countries, emphasizing the specific case of France, across various indicators. These graphs offer a visual representation of how France compares to other nations in key areas related to job conditions and satisfaction for the year 2018.  


![indicators](https://github.com/OsvaldoValdivia/P4-Job_satisfaction/blob/main/Images/indicators.gif)


### Variable map visuals

These maps visually illustrate the variations and differences among countries with regard to various indicators. Each indicator is color-coded on the map, allowing for a quick and intuitive understanding of how each country performs in relation to that specific variable.  


![maps](https://github.com/OsvaldoValdivia/P4-Job_satisfaction/blob/main/Images/maps.gif)


### Multivariable analysis

This series of graphs compares multiple countries using two-axis graphs. Each graph displays two different indicators, showing potential relationships between them. A Pearson correlation test has been conducted to quantify these relationships. This visual and statistical analysis helps uncover connections and trends in job conditions and satisfaction across countries.  


![multivariables_analysis](https://github.com/OsvaldoValdivia/P4-Job_satisfaction/blob/main/Images/multivariables_analysis.gif)


### Decision Tree (regression)

In essence, the decision tree in this project acts as a powerful analytical tool for exploring the complex relationships between socio-economic indicators and job satisfaction. It aids in building a model that provides insights into the influence of these indicators and their relative importance in determining job satisfaction across various European countries.


![decision_tree](https://github.com/OsvaldoValdivia/P4-Job_satisfaction/blob/main/Images/tree.png)

Indicators importance description

![indicators_importance](https://github.com/OsvaldoValdivia/P4-Job_satisfaction/blob/main/Images/indicators_importance.png)

### Conclusion

Based on the importance scores obtained from the decision tree analysis, we can draw several conclusions for the project regarding the socio-economic indicators and their influence on job satisfaction. Here's a conclusion based on the importance scores:

- Mean Net Income (MEAN_NET_INCOME): This indicator, with a substantial importance score of 0.49321, stands out as the most influential factor in explaining job satisfaction. Higher net income is strongly associated with increased job satisfaction, suggesting that financial well-being plays a crucial role in job satisfaction levels.

- Gender Pay Gap (GENDER_PAY_GAP): Although it has a relatively lower importance score (0.04323) compared to income, the gender pay gap is still noteworthy. A smaller gender pay gap contributes positively to job satisfaction, emphasizing the importance of gender equality in the workplace. This indicator must be carefully considered as the data we use in the project has no gender-distinction. This means we have not the information about the percentage of males and females.

- Inability to Handle Unexpected Expenses (INABILITY_UNEXPECTED_EXPENSES): With a score of 0.03004, this indicator suggests that the ability to manage unexpected financial burdens has a modest impact on job satisfaction. However, being financially prepared for unexpected expenses can contribute to higher job satisfaction.

- Working from Home (WORKING_HOME): This indicator, with a score of 0.03132, indicates that the option to work from home has a minor influence on job satisfaction. Flexibility in work arrangements, such as remote work, can contribute positively to overall job satisfaction. However this indicator may not only be limited to remote work but home work. As the datasource does not provide this information, we may carefully interpret this variable.

- Usually Working Evenings (USUALLY_WORKING_EVENING) and Sundays (USUALLY_WORKING_SUNDAYS): These indicators have limited importance scores (0.00244 and 0.00000, respectively), indicating that working evening hours and Sundays have a smaller impact on job satisfaction.

- Usually Working Saturdays (USUALLY_WORKING_SATURDAYS): This indicator holds the second most important position with an importance score of 0.27383. It plays a substantial role in influencing job satisfaction, highlighting the significance of the work schedule.

- Long Working Hours (LONG_WORKING_HOURS): Long working hours, while significant, have a lower importance score (0.12592) compared to income. This implies that job satisfaction is influenced by the number of extra hours worked, but other factors, particularly income, play a more dominant role.


In summary, the project's decision tree analysis reveals that income, is the most crucial factor in explaining job satisfaction. It significantly outweighs other indicators like the gender pay gap and the ability to handle unexpected expenses. The flexibility of working from home and working hours on evenings, Sundays have relatively minor impacts. This information can inform policies and strategies to enhance job satisfaction by focusing on income equality and work schedules.



## Datasets

The list of indicators extracted from Eurostat consists of data for job conditions and satisfaction-related variables from 33 European countries in the year 2018. These indicators are presented in a tabular format where each row represents a specific country, and each column represents a distinct job condition or satisfaction-related variable. The table offers valuable insights into the working conditions, job satisfaction, and well-being of individuals across Europe.

The data may include a wide range of indicators, such as average working hours, income levels, employment rates, job satisfaction ratings, the prevalence of long working hours, gender pay gap, evening work, and other relevant factors.


## Indicators description
 

A brief description of each indicator as well as the link to the data source is presented below. 

  

-  **AVG_WEEKLY_WORKING_HOURS** :

The indicator measures the average number of weekly working hours in individuals' primary jobs. This indicator's dataset contains merged data with the following filters : gender (males and females), age (15 to 64 years), employment status (employed persons), working time (full-time and part-time work), using the NACE Rev. 2 classification system. The data is reported annually and is expressed in hours.


<br> 


-  **LONG_WORKING_HOURS** :

The indicator "Long working hours" measures the prevalence of long working hours in individuals' primary jobs. This indicator's dataset contains merged data with the following filters :  gender (male and females), age (15 to 64 years), employment status (employed persons), using the International Standard Classification of Occupations 2008 (ISCO-08). The data is reported on an annual basis and is expressed as a percentage.



<br> 


-  **USUALLY_WORKING_EVENING** :

The indicator "Employed persons working in the evenings" measures the proportion of employed individuals who work in the evenings as part of their total employment. This indicator's dataset contains merged data with the following filters : gender (male and females), age (15 to 64 years), and employment status (employed persons). The information is reported on an annual basis and is expressed as a percentage.


<br> 


-  **MEAN_NET_INCOME** and **MEDIAN_NET_INCOME** :

This indicator reports the average and median income for different countries.  The indicator's data considers total income for both males and females, without gender-based distinctions in a population within the range of age of 16 - 64 years. The unit of measure is the euro.

 

<br> 


-  **FINANTIAL_SITUATION_RATING** :

The indicator "Satisfaction with finantial situation" provides a comprehensive view of satisfaction levels across different countries. The data is analyzed based on annual surveys and is filtered as follows: ages from 16 - 64 years, no male and female distinction. The rating goes from 0 - 10.


<br> 

-  **USUALLY_WORKING_SATURDAYS** and **USUALLY_WORKING_SUNDAYS** :

This indicator calculates the percentage of employed individuals who usually work on Saturdays as part of their total employment. The data is reported annually and is expressed as a percentage. The indicator presents no gender-based distinctions in a population within the range of age of 16 - 64 years.



<br> 



Links to the data sources

- AVG_WEEKLY_WORKING_HOURS : https://ec.europa.eu/eurostat/databrowser/view/LFSA_EWHUN2/default/table?lang=en. 
-  LONG_WORKING_HOURS : https://ec.europa.eu/eurostat/databrowser/view/LFSA_QOE_3A2$DV_608/default/table?lang=en.  
- USUALLY_WORKING_EVENING : https://ec.europa.eu/eurostat/databrowser/view/LFSA_EWPEVE$DV_604/default/table?lang=en.
- MEAN_NET_INCOME and MEDIAN_NET_INCOME : https://ec.europa.eu/eurostat/databrowser/view/LFSA_EWPEVE$DV_604/default/table?lang=en.
- FINANTIAL_SITUATION_RATING : https://ec.europa.eu/eurostat/databrowser/view/ILC_PW01$DV_524/default/table?lang=en.  
- USUALLY_WORKING_SATURDAYS : https://ec.europa.eu/eurostat/databrowser/view/LFSA_EWPSAT$DV_606/default/table?lang=en
- USUALLY_WORKING_SUNDAYS** : https://ec.europa.eu/eurostat/databrowser/view/LFSA_EWPSUN$DV_607/default/table?lang=en.