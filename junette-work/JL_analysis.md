Junette Lee\
NU-CHI-DATA-PT-12-2020-U-C\
07 Project One - Analysis\
Presentation Date: February 20, 2021

## Do we see a shift in consumption amount over decades?
* Both the year over year bar graphs of total consumption based on volume (gallons per capita) and based on total number of drinks (beer/wine/spirits) look very similar. This tells us that data is normalized to minimize potential skew resulting from varying alcohol contents in the measured beverage types (beer/wine/spirits).

    ![Annual Consumption by Volume](Images/JL%20-%20Annual%20US%20Ethanol%20Consumption%20Per%20Capita%20(1977-2018).png).
    ![Annual Consumption by Drink Count](Images/JL%20-%20Annual%20US%20Number%20of%20Drinks%20Per%20Capita%20(1977-2018).png).

* When viewing alcohol consumption by volume (gallons of ethanol), we observe a decrease in consumption over the past 30 years between 1977-2018.  However, the R-squared value is not high enought to prove any strong statistical correlation between time and alcohol consumption. The below visualization confirms our group's hypothesis that there would be a general decline in alcohol consumption over the past few decades. Since we begain this analysis with the assumption that many factors ranging from economic, environmental to social can all contribute to alcohol consumption, our goal was to observe any potential factors rather than to test one specific cause/effect.

    ![US Total Ethanol Consumption Per Capita, Bar](Images/JL%20-%20US%20Total%20Ethanol%20Consumption%20Per%20Capita,%20Bar%20(1977-2018).png).

## Is the shift in consumption consistent between alcohol types?
* After observing the overall trend of decline in consumption per capita, I wanted to examine if the decline was consistent between all measured alcohol types. With closer analysis, we see this is not the case. Beer consumption had a very strong R-squared (-0.94) and was strongly correlated to time. However, beer also made up about half of the total alcohol consumed so the combined consumption would be most affected by the beer data.
* The wine consumption saw increased consumption per capita contrary to beer, spirits, and the combined which all had negative regressions. Wine consumption also makes up the smallest percentage among the alcohol types measured, so the positive regression was hidden until we examined this more closely. The R-squared value (0.61) is not strong enough to prove causation, but we do see a slight shift in alcohol type preference via this calculation.
* Spirits consumption fluctuated the most out of the 3 alcohol types. We observe a wave where consumption starts off high, dips low, and rises again. The R-squared (-0.5) tells us there is no statistical significance between spirits consumption and time.

    ![US Total Ethanol Consumption Per Capita, Stacked](Images/JL%20-%20US%20Total%20Ethanol%20Consumption%20Per%20Capita,%20Stacked%20(1977-2018).png).
    ![US Total Ethanol Consumption Per Capita, Subplots](Images/JL%20-%20US%20Total%20Ethanol%20Consumption%20Per%20Capita,%20Subplots%20(1977-2018).png).
    ![Beer Consumption Per Capita](Images/JL%20-%20Beer%20Consumption%20Per%20Capita%20(1977-2018).png).
    ![Wine Consumption Per Capita](Images/JL%20-%20Wine%20Consumption%20Per%20Capita%20(1977-2018).png).
    ![Spirit Consumption Per Capita](Images/JL%20-%20Spirit%20Consumption%20Per%20Capita%20(1977-2018).png).

* When broken down by region (Northeast/Midwest/South/West), we observe each region following similar patterns in decrease and increase. Generally, the West Region consumed the most alcohol per capita and the South Region consumed the least per capita. Upon closer examination of regional populations we also see that as population increases, we see the inverse effect in alcohol consumption. The West Region had its higher per capita consumption when population was its lowest. Also, the South Region generally has the lowest per capita consumption but also had the highest population than any other region.
* This tells us that ouliers may be influencing the per capita consumption, especially when observing a smaller sample size. Outliers may include tourists consuming alcohol while vising a region where they do not live (e.g. California wine consumption).

    ![Regional Ethanol Consumption Per Capita](Images/JL%20-%20Regional%20Ethanol%20Consumption%20(1977-2018).png). 
    ![Regional Population Totals](Images/JL%20-%20Regional%20Population%20Totals%20(1977-2018).png).
    
## Cleaning the data
* I found early on that the NIH NIAAA dataset used Census population data as well as CDC Wonder Race-Bridged Population Estimates for population values. This helped us align any additional population data from additional sources to the same age parameters (14 years and older) already factored into the per capita NIAAA data calculations.