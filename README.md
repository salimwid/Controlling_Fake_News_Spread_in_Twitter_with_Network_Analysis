# Controlling_Fake_News_Spread_in_Twitter_with_Network_Analysis
[Python] Proposed end-to-end (E2E) network analysis process needed to disrupt the spread of fake news by limiting the activity of infected nodes.

### Models Deployed
Community Detection (Leading Eigenvector, Asynchoronous Label Propagation, Fluid Communities, Kernighan Lin Maximization), Random and Targeted Network Attacks

### Techniques Employed
Exploratory Data Analysis, Feature Engineering, Data Visualization, Network Analysis, Distributed Network Disruption, Community Detection, Big Data Processing

### Tools Employed
iGraph, sklearn, seaborn, pyplot, graphframes, networkx, pyspark, Tigergraph, MapReduce

### Context
Financial offshoring activity is a worldwide phenomenon. While some of these activities are done under a legal context, many have been discovered to lean towards criminal activities such as money laundering, tax evasion and fraud. The tangible costs of these activities are colossal; it is estimated that countries worldwide lose over USD$4271 billion in tax each year due to tax evasion and abuse. Multinational corporations shifted more than USD$650 billion – about 40% of their profit – worth of profit into tax havens, while private tax evaders stored more than USD$10 trillion in financial assets offshore to avoid paying taxes. The social costs are also exigent, lower-income countries’ tax losses are equivalent to nearly 52% of their combined public health budget. <br>

Many governments are now willing to cooperate to combat offshoring by imposing region-wide sanctions or residual tax payments towards tax havens. However, these policies still fall short – recovering only 0.4% of the annual offshoring costs. This project used network analytics methodologies to construct and analyse the global offshoring network contained in the Offshore Leaks papers. <br>

The Offshore Leaks papers span over 80 years and contain relationships between more than 200 countries and territories worldwide. The key objectives of this project are: (1) To discover global offshoring network structures and behaviours; (2) To explore and test the network’s resilience; and (3) To identify the top countries and financial regions.

### Datasets
The FakeNewsNet dataset was utilized - more specifically, the Politifact subset. The original dataset were consisted of data from user and news. We processed the data and came up with Tweets and Followers data which contained 573,637 unique users with more than 1 billion potential follower-followee matrix interactions. <br>

We found that in the dataset, there were 779 news (47% was fake news), 544,027 tweets (28% was fake news) and 68,099 retweets (27% retweeted fake news).

### Network Formation & Methodology
From the initial dataset, 2 network structures were created with the following objectives: <br>
(1) <strong> Tweet-Retweet Network </strong> which was explored to target community based on retweeting connections. <br>

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
Gino Tiu <br>
Widya Salim <br>
Felipe Chapa <br>
Susan Koruthu
