# LCA Model - Natural Gas Transportation - GREET

<h2>Description</h2>
This is a simple LCA that calculates the carbon footprint in the transportation of natural gas through pipelines and as LNG employing the GREET model. 
<br />

<h2>Tools/Applications Used</h2>

- <b>GREET</b> 

<h2>Introduction</h2>

[Greenhouse Gases Regulated Emissions and Energy Use in Transportation](https://greet.anl.gov/files/2011ws-overview-lca) aka the GREET model was developed in 1996 by the Argonne National Laboratory. The GREET LCA model uses more than 100+ fuel production pathways from various energy feedstocks. It measures the inputs, outputs, and environmental impacts of a fuel product system throughout its lifecycle (well to wheels). 

<p align="center">
<br/>
<a href="https://imgur.com/wWc22r8"><img src="https://i.imgur.com/wWc22r8.jpg" alt="Fuel and Vehicle Cycle (GREET)" /></a> 
</p>

The GREET model works by defining the product and its production system, determining the inputs and outputs of such a system, which are products, materials, and energy, and then simulating processes that convert input to output.

<p align="center">
<br/>
<a href="https://imgur.com/zorhZ1A"><img src="https://i.imgur.com/zorhZ1A.png" alt="Natural Gas Production and Delivery" /></a> 
</p>

<h2>Goal and scope definition:</h2>

For our purposes, we’ll be simulating a version of well-to-pump fuel cycle for the comparison between LNG and pipelines as the GREET model specifically caters to the LCA of fuel in transportation and not exactly fuel transportation, and consequently the consumption and end-of-life phase. The GREET model especially utilizes EPA methodologies and data, for performing GHG analysis of specific energy systems. This document covers two simulations using the GREET model:
1. Transportation of natural gas from a location in North America to an export terminal in Louisiana (using pipelines)
2. Liquefaction of natural gas and transportation from Louisiana to Germany (using LNG tanker)

<h2>Inventory Analysis:</h2>

The inventory analysis is limited to the following stages:
1. Raw Material Production
2. Process of manufacturing and production
3. Distribution and Transportation

Out of the above, we'll be especially looking into the calculation of the emissions in the third stage - distribution and transportation from the GREET model.

<b>Transportation of natural gas from a location in North America to an export terminal in Louisiana (using pipelines)</b>

This process is designed in the GREET Model in three steps which are as follows:
a) Setting up the transportation process of Natural Gas from a Natural Gas field in North America (say Keystone, PA) to an export terminal in Louisiana (say Plaquemines LNG, LA). The distance between the two is roughly 1180 miles which is set as parameters.

<p align="center">
<br/>
<a href="https://imgur.com/zh5Q29j"><img src="https://i.imgur.com/zh5Q29j.png" alt="Natural Gas transportation through pipelines" /></a>
</p>

b) Setting up the pathway of the process comprising of two processes: 
i) Stationary process of the production of natural gas from a North American Natural Gas field (in our case the Keystone PA).
ii) Transportation process (that we created in Step 1) for the transportation of the natural gas from Keystone, PA to Plaquemines, LA).

<p align="center">
<br/>
<a href="https://imgur.com/zCFtW8E"><img src="https://i.imgur.com/zCFtW8E.png" alt="Pathway of Natural Gas transportation" /></a>
</p>

c) Calculating the results in the ‘WTP Results’ pane by selecting the pathway created in Step 2.

<p align="center">
<br/>
<a href="https://imgur.com/2N9h2lk"><img src="https://i.imgur.com/2N9h2lk.png" alt="WTP Results Natural Gas through pipelines" /></a>
</p>

<h2>Impact Assessment:</h2>

<p align="center">
<br/>
<a href="https://imgur.com/v9tGdzn"><img src="https://i.imgur.com/v9tGdzn.jpg" alt="Basic Solar Finance Model" /></a>
</p>

<h2>Interpretation:</h2>

<p align="center">
<br/>
<a href="https://imgur.com/v9tGdzn"><img src="https://i.imgur.com/v9tGdzn.jpg" alt="Basic Solar Finance Model" /></a>
</p>


<h2>References:</h2>

<p align="center">
<br/>
<a href="https://imgur.com/v9tGdzn"><img src="https://i.imgur.com/v9tGdzn.jpg" alt="Basic Solar Finance Model" /></a>
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
