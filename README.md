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

This process is designed in the GREET Model in three steps which are as follows:<br/>
a) Setting up the transportation process of Natural Gas from a Natural Gas field in North America (say Keystone, PA) to an export terminal in Louisiana (say Plaquemines LNG, LA). The distance between the two is roughly 1180 miles which is set as parameters.

<p align="center">
<br/>
<a href="https://imgur.com/zh5Q29j"><img src="https://i.imgur.com/zh5Q29j.png" alt="Natural Gas transportation through pipelines" /></a>
</p>

b) Setting up the pathway of the process comprising of two processes: <br/>
i) Stationary process of the production of natural gas from a North American Natural Gas field (in our case the Keystone PA).<br/>
ii) Transportation process (that we created in Step 1) for the transportation of the natural gas from Keystone, PA to Plaquemines, LA).<br/>

<p align="center">
<br/>
<a href="https://imgur.com/zCFtW8E"><img src="https://i.imgur.com/zCFtW8E.png" alt="Pathway of Natural Gas transportation" /></a>
</p>

c) Calculate the results in the ‘WTP Results’ pane by selecting the pathway created in Step 2.

<p align="center">
<br/>
<a href="https://imgur.com/2N9h2lk"><img src="https://i.imgur.com/2N9h2lk.png" alt="WTP Results - Natural Gas through pipelines" /></a>
</p>

<b>Liquefaction of natural gas and transportation from Louisiana to Germany (using LNG tanker)</b>

This process is designed in the GREET Model in three steps which are as follows:<br/>
a) Setting up the transportation process from Plaquemines LNG plant, Louisiana to LNG import terminal in Germany (say Hamburg, Germany). The distance between the two is roughly 5000 miles which is set as parameters.

<p align="center">
<br/>
<a href="https://imgur.com/h9cQ8sh"><img src="https://i.imgur.com/h9cQ8sh.png" alt="Natural Gas transportation as LNG" /></a> 
</p>

b) Setting up the pathway comprising of four processes/pathways (as shown in Fig 6):<br/>
i) Pathway of the production and transportation of natural gas from a natural gas field in Keystone, PA to LNG export terminal in Plaquemines, LA (from Simulation 1 above).<br/>
ii) Stationary process of Liquefaction of Natural Gas into Liquefied Natural Gas in the Plaquemines LNG plant, LA.<br/>
iii) Transportation process (that we created in Step a) for the transportation of the liquefied natural gas from Plaquemines, LA to LNG terminal in Hamburg, Germany.<br/>
iv) Stationary process of regasification of liquefied natural gas to natural gas.<br/>

<p align="center">
<br/>
<a href="https://imgur.com/ei1bSJy"><img src="https://i.imgur.com/ei1bSJy.png" alt="Pathway of LNG transportation" /></a>
</p>

c) Calculate the results in the ‘WTP Results’ pane by selecting the pathway created in Step 2.<br/>

<p align="center">
<br/>
<a href="https://imgur.com/jxjui8F"><img src="https://i.imgur.com/jxjui8F.png" alt="WTP Results - Natural Gas as LNG" /></a>
</p>

<h2>Impact Assessment (CO2 Total Emissions):</h2>

<b>Transportation of natural gas from a location in North America to an export terminal in Louisiana (using pipelines)</b>
1. NG from Shale and Conventional Recovery - 4.3686 kg
2. Pathway - NG pipeline from PA to LA - 10.1094 kg
3. Emissions & Resource Use in pipeline transportation (2-1) - 5.7408 kg

<b>Transportation of natural gas from a location in North America to an export terminal in Louisiana (using pipelines)</b>
1. Pathway - NG pipeline from PA to LA -> 10.1094 kg
2. NG Liquefaction as an intermediate fuel -> 16.6598 kg
3. LNG Transportation via ocean tanker from Louisiana to Germany -> 17.7893 kg
4. LNG to NG via liquid evaporation in heat exchanges -> 17.7893 kg
5. Pathway - NG pipeline from Hamburg to Berlin, Germany -> 18.7623 kg
6. Isolated emissions from LNG liquefaction process (2-1) -> 6.5504 kg
7. Isolated emissions from LNG transportation from LA to Germany (3-2) -> 1.1295 kg
8. Isolated emissions from LNG regasification to NG (4-3)	-> 0 kg
9. Isolated emissions from NG transportation from Hamburg to Berlin (5-4) -> 0.973 kg
10. Total isolated emissions from LNG transportation -> 8.6529 kg

<h2>Interpretation:</h2>

1. As seen in LNG transportation, the gasification process is emissions intensive with 6.5504 kg.
2. Compared to pipelines, LNG tankers have fewer emissions as a transportation medium (1.1295 kg)
3. LNG is, therefore, a better alternative over large distances, compared to pipelines.

<h2>References:</h2>

<b>•	https://www.energy.gov/sites/prod/files/2014/02/f8/HS_NatGas_Studyguide_draft2.pdf</b><br/>
<b>•	https://www.eia.gov/energyexplained/natural-gas/where-our-natural-gas-comes-from.php</b>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
