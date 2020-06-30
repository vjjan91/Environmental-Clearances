# Environmental Clearances 
This repository contains data, scripts and figures pertaining to environmental clearances (as obtained from the PARIVESH portal hosted by the MOEF&amp;CC)

## So what's this repository about?

We obtained and analyzed the raw data on clearances from [PARIVESH](http://parivesh.nic.in/), a portal hosted by the MOEF&CC. A summary of the analysis follows. However, all data, figures and scripts emerging from the exploratory data analysis can be obtained from the respective folders.

## Data on Environmental Clearances

Environmental clearance data is organized under three sub-headings on the PARIVESH portal, hosted by the MOEF&CC. These include: Environmental, Forests and Wildlife. The data for Forests and Wildlife are quantifiable, while the data for 'Environmental clearances' does not have any quantifiable information associated with it. In other words, these proposals lack any information on the area of forests stated to be cleared. At present, data for forests are available as an excel file on the portal (albeit, after much digging and searching). Data for Wildlife clearances was not available as an excel file. 

All analysis was performed through the R programming environment. Please feel free to edit and use the code as you please. The data used for this purpose is available through the 'Data' folder. 

### How did we categorize and analyze the data?

In 1994, the Union Ministry of Environment and Forests (MEF), Government of India, under the Environmental (Protection) Act 1986, promulgated an EIA notification making Environmental Clearance (EC) mandatory for expansion or modernisation of any activity or for setting up new projects listed in Schedule 1 of the notification. A decade later, a new EIA legislation was passed in 2006. However, unlike the EIA Notification of 1994, the new legislation has put the onus of clearing projects on the state government depending on the size/capacity of the project. Click [here](https://www.cseindia.org/understanding-eia-383#:~:text=On%2027%20January%201994%2C%20the,listed%20in%20Schedule%201%20of)for more details. 

Based on the above information, we reran the analyses by binning clearances across three time periods: 2000 to 2006; 2007 to 2014 and 2014 to Present.

### Forest Clearances

The data on forest clearances has been stored in 5 separate excel files:

1. All data prior to 2014
2. Data post 2014 is subdivided by the MOEF&CC into:  
    a) Allocation of fresh forest land (Form-A)	   
    b) Application Under Section 2(iii)	     
    c) Renewal of lease (Form-B)         	  
    d) Prospecting of Minerals (Form-C)    

For the sake of the analysis, we clubbed the above four categories into a single category on clearances post 2014. Secondly, the analysis only includes area in hectares across those proposals that have been categorized as currently approved / pending to be approved (*See code for further details*).

**Between 2000 and 2006, 5076 proposals were categorized as approved / under one of the pending categories. During the same period, 1213 proposals were rejected. 
Proportion of proposals rejected: 19.3%**

**Between 2007 and 2014, 9829 proposals were categorized as approved / under one of the pending categories. During the same period, 1161 proposals were rejected. 
Proportion of proposals rejected: 10.5%**

**Between 2014 and 2020, 17037 proposals were categorized as approved / under one of the pending categories. During the same period, 120 proposals were rejected. 
Proportion of proposals rejected: 0.7%!**

If we look at the above information in terms of area:

**2000 to 2006: Area stated to be cleared / potentially cleared - 6,29,638 hectares**
**2000 to 2006: Area saved - 2,54,555.6 hectares**

**2007 to 2014: Area stated to be cleared / potentially cleared - 4,51,676 hectares**
**2007 to 2014: Area saved - 41,556.63 hectares**

**2014 to Present: Area stated to be cleared / potentially cleared - 14,82,247 hectares**
**2014 to Present: Area saved - 13,077.03 hectares**

Between 2000 and 2006, Majority of area stated to be cleared was towards mining projects 

![Area by Category 2000-2006](https://github.com/vjjan91/Environmental-Clearances/blob/master/Figures/cat_area_2000-2006.png)

A similar trend towards mining projects was seen between 2007 and 2014.

![Area by Category 2007-2014](https://github.com/vjjan91/Environmental-Clearances/blob/master/Figures/cat_area_2007-2014.png)

When compared to the previous time period, area under mining has ** increased six-fold** between 2014 to 2020.

![Area by Category post 2014](https://github.com/vjjan91/WithdrawEIA2020/blob/master/Figures/post2014_Area_vs_Category.png)

2006 is an outlier year that has seen large chunks of forested land approved for clearing

![Area by Year 2000-2006](https://github.com/vjjan91/Environmental-Clearances/blob/master/Figures/year_area_2000-2006.png)

![Area by Year 2007-2014](https://github.com/vjjan91/Environmental-Clearances/blob/master/Figures/year_area_2007-2014.png)

Post 2014, large chunks of forested land were approved for clearing in the year 2016. Notice, that **the amount of forest area approved for clearing in 2016 was more than double the amount of forest area approved for clearing in 2006 alone.** 

![Area by Year post 2014](https://github.com/vjjan91/WithdrawEIA2020/blob/master/Figures/post2014_Area_by_Year.png)

Between 2000 and 2006, a large area of forests were approved/pending to be cleared in Madhya Pradesh followed by Arunachal Pradesh - two states that possess an astounding level of biodiversity.

![Area by State 2000 2006](https://github.com/vjjan91/Environmental-Clearances/blob/master/Figures/state_area_2000-2006.png)

A similar trend was seen between 2007 and 2014 for the state of Arunachal Pradesh

![Area by State 2007 2014](https://github.com/vjjan91/Environmental-Clearances/blob/master/Figures/state_area_2007-2014.png)

Post 2014, Andhra Pradesh and Telangana are stated to lose the most chunks of forest land. 

![Area by State post 2014](https://github.com/vjjan91/WithdrawEIA2020/blob/master/Figures/post2014_Area_by_State.png)

A map of area of forests approved/pending to be cleared (post 2014)

![Area by State post 2014 map](https://github.com/vjjan91/WithdrawEIA2020/blob/master/Figures/state_area_post2014.png)

**The analysis suggests that there has been a significant increase in the rate of environmental clearances for the forest category alone since 2014. Further, the proportion of proposals rejected since 2014 is less than 1%.**

*For further analysis on area lost by category by state across two time periods, please visit the figures folder*



