
<h1>Analysis of COVID impact on US households</h1>

Lakshmi Venkatasubramanian 
12/9/2020

<h3> Motivation </h3> 

<p>The goal of this analysis is to gauge the impact of the pandemic on overall household characteristics such as employment status, housing, education disruptions, and dimensions of physical and mental wellness. There is a large amount of emotionally negative stimuli related to the COVID-19 pandemic. How do people prepare themselves in difficult times like this? Analyzing and exploring people's response to pandemic can provide useful insights into people's perspective about COVID and the challenges they face.</p>

<p>As we all know,the impacts of the pandemic and the economic fallout have been widespread, but are particularly prevalent among Black, Latino, Indigenous, and immigrant households. This analysis will  deep dive into some of the impacts of covid by Age group, race and ethinicity. We also try to understand the different groups of people based on various characteristics who have been impacted by COVID. The research questions will follow quantitative analysis and will target specific variables. Below are some references: </p>
<li><a href='https://www.cbpp.org/research/poverty-and-inequality/tracking-the-covid-19-recessions-effects-on-food-housing-and'>Covid Recession effects</a></li>
<li><a href='https://www.cdc.gov/nchs/covid19/pulse/mental-health.htm'>Covid data from NCHS</a></li>


## Repository structure
```
├── README.md
├── LICENSE
├── assets
│   └── pictures
├── clean_data
│   ├── covid_clean_data.csv
├── raw_data
│   └── raw.csv
└── src
    ├── Analysis of COVID impact on US households.ipynb
    ├── COVID_impact_cleaning_data.ipynb
```

<h3>Data Source</h3>
<p>The <a href='https://www2.census.gov/programs-surveys/demo/technical-documentation/hhp/2020_HPS_Background.pdf'>Household Pulse Survey</a> provides timely data to help understand the experiences of American households during the coronavirus pandemic. Data for this research comes from the Phase 1 Household Pulse Survey that began on April 23 and ended on July 21, 2020. The dataset is very rich and informative. It dataset has 105 variables, 1088314 observations and includes employment status, food security, housing, physical and mental health, access to health care, and educational disruption. In order to support the nation’s recovery, we need to know the ways this pandemic has affected people’s lives and livelihoods. Data from these datasets will show the widespread effects of the coronavirus pandemic on individuals, families, and communities across the country. </p>

<p>The survey was conducted by an internet questionnaire, with invitations to participate sent by email and text message. Housing units linked to one or more email addresses or cell phone numbers were randomly selected to participate, and one respondent from each housing unit was selected to respond.</p>

<h4> Links to Data set and Data dictionary</h4>
<ul><li>The datasets are available for public use under <a href='https://www.census.gov/programs-surveys/household-pulse-survey/datasets.html'>census.gov</a> website as weekly files.</li>
<li>Data dictionary is available in the census.gov website under the link <a href='https://www.census.gov/programs-surveys/household-pulse-survey/technical-documentation.html#phase1'>Phase 1 Household Pulse Survey Technical Documentation</a></li></ul>

<h4>Download data</h4>
<p>Data is directly downloaded from census website using zipfile package<p>
  

<h4>Terms of use of census data </h4>
<p>The Census Bureau is committed to open government by sharing its public data as open data. Census data continues to be a key national resource, serving as a fuel for entrepreneurship and innovation, scientific discovery, and commercial activity.  We continuously identify and publish datasets and Application Programming Interface’s (API’s) to Data.gov in accordance with the Office of Management and Budget (OMB) Memorandum M-10-06, the Executive Order 13642 on open data, and the overall principles outlined in the Digital Government Strategy.  In
 accordance with the Open Data Policy, M-13-13, the Census Bureau publishes its information in machine-readable formats while also safeguarding privacy and security.</p>

<h3>Research Questions</h3>
<ul>
    <li>Understand the impacts of COVID in terms of employment loss, income loss, food insufficiency, education interruptions, inability to meet housing expenses and how does this vary by Race/Ethnicity or gender? Are minority groups and women affected the most?</li>
    <li>What is the impact on physical and mental wellness? Is there a correlation between Anxiety and depression and factors such as age, number of household members, income, health status, race, gender? How does the anxiety levels vary between first and last week of survey?</li>
    <li>How does employment loss, income loss, food insufficiency, education interruptions, inability to meet housing expenses in Washington differ as compared to other states?</li>
    <li>How do different groups based on age, race and ethnicity differ in their behavior or attitude towards COVID. Are there any patterns observed in the population based on certain characteristics pertaining to COVID?</li> 
</ul>


<h3>Methodology</h3>
<p>For all the research questions, multivariate analysis will be used.</p>
<p><strong>Statistical Analysis Method</strong>
<ul><li>Regression analysis will be used to train and determine the impactful predictors. This method is appropriate as all the data points are independent and the sample size is large enough to meet the normality assumption. As the dataset has both numerical and categorical data, regression techniques are suitable. The model is also interpretable.</li>
<li>k-means clustering will be used to identify any patterns and classify groups of people based on similar characteristics</li></ul></p>
<p><strong>Results</strong>
    <li>The results will be presented in a comprehensive compilation of visualizations.</li>
</p>

<h3>Source of Bias</h3>
<p> Nonsampling errors can also occur and are more likely for surveys that are implemented quickly, achieve low response rates, and rely on online response.  Nonsampling errors for the Household Pulse Survey may include:</p>

<ul><li><strong>Measurement error:</strong> The respondent provides incorrect information, or an unclear survey question is misunderstood by the respondent. The Household Pulse Survey schedule offered only limited time for testing questions. </li>
<li><strong>Coverage error: </strong>Individuals who otherwise would have been included in the survey frame were missed. The Household Pulse Survey only recruited households for which an email address or cell phone number could be identified.</li>
<li><strong>Nonresponse error:</strong> Responses are not collected from all those in the sample or the respondent is unwilling to provide information. The response rate for the Household Pulse Survey was substantially lower than most federally sponsored surveys.</li>
<li><strong>Processing error: </strong>Forms may be lost, data may be incorrectly keyed, coded, or recoded. The real-time dissemination of the Household Pulse Survey provided limited time to identify and fix processing errors.</li></ul>
 
<p>The Census Bureau employs quality control procedures to minimize these errors.  However, the potential bias due to nonsampling errors has not yet been evaluated.</p>


<h3>Resources used</h3>

This analysis was prepared using Python 3.8 running in a Jupyter Notebook environment.  
Documentation for Python can be found here: https://docs.python.org/3.8/  
Documentation for Jupyter Notebook can be found here: http://jupyter-notebook.readthedocs.io/en/latest/  

The following Python packages were used and their documentation can be found at the accompanying links:

* [pandas](https://pandas.pydata.org/)
* [numpy](https://numpy.org/)
* [IPython](https://ipython.org/)
* [matplotlib](https://matplotlib.org/)
* [seaborn](https://seaborn.pydata.org/)

<h3>Unknowns and dependencies</h3>
<p>These data are experimental and samples may not be representative of the population. </p>



