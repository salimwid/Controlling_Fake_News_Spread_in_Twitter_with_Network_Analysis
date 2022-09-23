# Controlling_Fake_News_Spread_in_Twitter_with_Network_Analysis
[Python] This project used network analytics methodologies to construct and analyse the global offshoring network contained in the Offshore Leaks papers.

### Models Deployed
Community Detection (Spinglass and Leading Eigenvector), Random and Targeted Network Attacks, Chord Diagram

### Techniques Employed
Exploratory Data Analysis, Feature Engineering, Data Visualization, Network Analysis, Distributed Network Disruption, Community Detection

### Tools Employed
iGraph, sklearn, seaborn, plotly

### Context
Financial offshoring activity is a worldwide phenomenon. While some of these activities are done under a legal context, many have been discovered to lean towards criminal activities such as money laundering, tax evasion and fraud. The tangible costs of these activities are colossal; it is estimated that countries worldwide lose over USD$4271 billion in tax each year due to tax evasion and abuse. Multinational corporations shifted more than USD$650 billion – about 40% of their profit – worth of profit into tax havens, while private tax evaders stored more than USD$10 trillion in financial assets offshore to avoid paying taxes. The social costs are also exigent, lower-income countries’ tax losses are equivalent to nearly 52% of their combined public health budget. <br>

Many governments are now willing to cooperate to combat offshoring by imposing region-wide sanctions or residual tax payments towards tax havens. However, these policies still fall short – recovering only 0.4% of the annual offshoring costs. This project used network analytics methodologies to construct and analyse the global offshoring network contained in the Offshore Leaks papers. <br>

The Offshore Leaks papers span over 80 years and contain relationships between more than 200 countries and territories worldwide. The key objectives of this project are: (1) To discover global offshoring network structures and behaviours; (2) To explore and test the network’s resilience; and (3) To identify the top countries and financial regions.

### Datasets
The dataset was acquired from the ICIJ Panama Papers Offshore Leaks Database and contained information from all of the Offshore Leaks papers. There were 5 Offshore Leaks papers: Offshore Leaks (2013), Panama Papers (2016), Bahamas Leaks (2016), Paradise Leaks (2017) and Pandora Papers (2021). Each paper contained information on more than 100,000 entities or individuals along with their links to large intermediaries, offshore providers or law firms. The papers have a coverage of more than 200 countries. The dataset acquired combined entries from the aforementioned papers into 4 tables: Entities, Intermediaries, Officers and Relationships. To construct the network, we assigned countries to become nodes while the edges are the relationships that these countries have with each other. <br>

The final dataset contains 196 countries or independent states with 338,124 unique edges and 5 relationship types that were weighted based on importance to the network. For this study, a directed network was adopted since identifying capital inflow and outflow between countries is key to understanding offshoring behaviours.

### Chosen Model
For community detection, spinglass and leading Eigenvector were chosen because they gave the most number of insightful clusters. Meanwhile, for network attacks and degradation, random and targeted attacks were simulated to understand how robust the network.
<br>

### Insights & Impact
Several interesting insights were found: <br>
<li> In Latin America, most offshoring activities were in fact, onshoring, from this region into Panama. Panama was chosen as it was a territory which is “local, culturally similar, and socially-linked” to Central and South America.</li> <br>
<li> Top ranked territories were further classified into four metric-rank groups: Hub Territories (HT), Authority Territories (AT), Highly Active Territories (HAT) and Bridging Territories (BT).</li> <br>
<li> Southeast Asian countries have a high weighted out-degree in no intermediary network. This suggests that most offshoring activities in these regions are done directly by private individuals.</li> <br>
<li> The offshoring network is quite resilient to random edge attacks, it needs up to more than 40% of edges removed before it starts failing. This reflects the real world scenario where authorities spend a lot of resources to prosecute individuals and/or entities with minimal impact.</li><br>
<li> When the typical tax haven territories (e.g: Caribbean) are removed, the remaining tax haven territories are: (a) highly active offshoring countries like United Kingdom and China; and (b) capital rich tax haven territories like Singapore and Ireland. Removal of these territories in the network is more effective than randomly removing edges as they are 'transit hub' for offshoring activities.</li> <br>

These findings highlight certain considerations for policymakers: <br>
(1) Impose localised policy based on the region’s offshoring behaviours. <br>
(2) Focus on highly active territories might be needed to disrupt the network. <br>
(3) Tax haven territories should be differentiated between capital rich versus offshoring bases. <br>
(4) Preventive policies should focus on cooperation and restraining activities between countries rather than targeting individuals.

### Collaborators
Susan Koruthu <br>
Widya Salim <br>
Hpone Myat Khine <br>
Sae Jin Jang
