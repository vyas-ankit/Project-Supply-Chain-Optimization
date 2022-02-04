Case Study - A Brief Overview

The case study aims at optimizing the supply chain network for a glass manufacturer in the United States. The company currently serves 50 customers located across the US, each of which has demand for five different glass products. The glass products are made at four different US plants. Currently, the company produces each product at one location only and serves each customer directly from the source plant.

The manufacturer is experiencing two major problems at the moment:

1) service to some distant customers has been unreliable and
1) rising gas prices have had a large impact on the balance sheet through transportation costs.

The manufacturer wants to explore2 options(eitherindividually orin tandem) toimprovetheservice and decrease transportation costs:

1) build warehouses
1) upgrade plants

Opex Analytics - Consulting Solutions

The consulting team at Opex Analytics has been tasked with building a model to help the CEO determine if either of these two changes should be made. In order to do this, we will need to use the model to determine how the proposed changes to the supply chain wouldaffect performancerelative to the current state.

Mathematical Modeling

The mathematical model is defined as a mixed-integer programming problem. The 2 options - building of warehouses and upgradation of plants - are analysed individually as well as in tandem.

In all, a total of 4 configurations are analysed whose results and codes are available in the .zip file:



|Configuration A|Current state of the SC|Sub-optimal Configurations|
| - | - | :- |
|Configuration B|Only warehouses are built||
|Configuration C|Only the plants are upgraded||
|Configuration D|Warehouses are built and plants are upgraded|Recommended Solution|
About the programming aspect of the model:

1) The model is built using the Pulp library in Python 3.5.
1) CBC solver is used to find the solutions.
1) All the codes are run on Macbook Pro 2.3 GHz Intel Core i5, anddonot takemorethan 10 mins to produce the results and write the solution to excel files.

The results in brief, for the 4 configurations are as follows:



||Profit (Million USD)|Transportation Cost (Million USD)|Service %|No. of warehouses|
| :- | :- | :- | - | :- |
|Conf. A|143|98|11|0|
|Conf. B|135|108|80|6|
|Conf. C|187|54|43|0|
|Conf. D|181|59|80|3|
Opex\_Case\_Study\_Sol.zip

The .zip file contains 4 folders:

1. Read Me

It contains 4 files:

1) Case Study - Problem Statement.pdf

It contains the complete description of the problem statement, objectives and deliverables.

2) Opex Case Study Write-up.pdf The current file.
2) Code Run.pdf

Contains information on changes to be made to run the code.

4) 1316\_Network\_Planning.xlsx

The file which contains data supplied to the optimisation model.

2. Presentation

It contains one .pdf file - ​*“Opex Case Study PPT - Ankit, 25\_10\_2020.pdf”* to be delivered before the CEO, senior-management and technical experts.

3. Codes

It contains 4 Jupyter Notebooks.

1) Conf. A - Current SC.ipynb

It contains the profit/cost analysis of the SC in the current state.

2) Conf. B - Only\_Warehouses.ipynb

It contains the profit/cost analysis when only warehouses are built in the SC.

3) Conf. C - Only\_Plant\_upgrades.ipynb

It contains the profit/cost analysis when only the plants are upgraded.

4) Conf. D - Plant\_Upgrade\_and\_Warehouses.ipynb

It contains the profit/cost analysis when plants are upgraded and warehouses are built in the SC.

Each notebook has the following results printed in it:

1) No. of warehouses to be built and their locations
1) Product assignments - which product are produced at which plant and in what quantities.
1) Total cost, revenue, profits
1) Break-up of total cost into transportation, changeover and production cost
1) Breakup of transportation cost into Plant → Customer, Plant → Warehouse and Warehouse → Customer shipping cost.
1) Service % (\*Service = % of total demand met by a facility within 500 mi of the customer )
1) Upgradation decision for each plant

viii) Changeover (set-up) decisions between the products at each plant

4. Result Files

It contains 4 excel files, each corresponding to one of the 4 configurations. Each excel file contains the following sheets:

1) Balance Sheet

It contains the overall values for costs, revenues and profits.

2) Total costs Breakup

It contains thebreak-upoftotal cost intotransportation cost, changeovercost andproduction cost.

3) Transportation Costs Breakup

It breaks up the transportation cost into 3 components:

Plant → Customer, Plant → Warehouse and Warehouse → Customer shipping cost

4) Product Assignments

It identifies which product is produced at which plant.

5) Production Quantities

It gives the quantity of a product produced at a given plant.

6) Qty - Plants to Warehouse
6) Qty - Plants to Customer

viii) Qty - Warehouse to Customer

These 3 sheetsidentify thequantitiesofeachproduct transportedfromPlants→Warehouses, Plants → Customers and Warehouses → Customers respectively.
