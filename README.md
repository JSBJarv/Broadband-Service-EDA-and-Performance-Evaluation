# Broadband-Service-EDA-and-Performance-Evaluation

## Overview
- Capture trends and insights by visualizing the variables and distribution of service providers, technology, tiers and KPI for broadband services in different states of Australia.
- Applied multiple logistic regression to classify the connection as impaired or underperforming based on KPI. Determine the values of download speed, upload speed and latency to let individual test their connection if impaired or underperforming.
- Implemented K-Means clustering to segment broadband services based on performance and variables.

### Exploratory Data Analysis
#### Observations
There are lots of observations we can get from the visualization and for the sake of this project not being too lengthy, we will only be taking notes of those who tops in the comparison.

<p align="center">
<img src="https://github.com/JSBJarv/Broadband-Service-EDA-and-Performance-Evaluation/blob/main/MBA%20Data%20Analysis.png" width="450" height="300">
</p>

#### RSP vs. Technology
- Aussie Broadband, Telstra and iNet are the major providers of Fiber to the Node connection.
- Hybrid Fibre Coaxial and Fiber to the Premises are second preferred connection which number varies depending on the service provider. iNet tops the chart in providing Fiber to the premises while TPG tops in Hybrid Fiber Coaxial.
- Fiber to the curb has the lowest number of subscribers which is also understandable due to the fact that out of these four, it has the least speed ceiling for both upload and download.

#### RSP vs. Tier
- Telstra is our top provider of 50/20 Mbps connection which also offers 100/20 Mbps as it ranks second behind Dodo & iPrimus.
- Observations also tell that Aussie Broadband still offers 25/10 Mbps.
- Launtel offers 250/100 Mbps and tops the other providers in servicing 400/50 Mbps even though it does not have a lot of subscribers in other tiers.

#### RSP vs. State
- TPG, Optus and Telstra are the top three RSP in New South Wales (NSW) while Aussie Broadband tops in providing internet connection in Victoria State.

#### RSP vs. Geography
- It is not a surprise that majority of RSP caters internet subscription in urban and residential areas.


### Performance Classification using Multiple Logistic Regression
In this section, we will be utilizing the is_this_service_impaired and is_this_service_underperforming to classify the value of our metrics. We will be using Multiple Logistic Regression to determine the have some expectation of our classification based on the value of the KPI metric by having the the recorded observation's corresponding probability.

<p align="center">
<img src="https://github.com/JSBJarv/Broadband-Service-EDA-and-Performance-Evaluation/blob/main/MBA%20Impaired%20Accuracy.png" width="450" height="300"> <img src="https://github.com/JSBJarv/Broadband-Service-EDA-and-Performance-Evaluation/blob/main/MBA%20Underperform%20Accuracy.png" width="450" height="300">
</p>
