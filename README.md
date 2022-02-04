 Case Study - A Brief Overview
The case study aims at optimizing the supply chain network for a glass manufacturer in the United States. The company currently serves 50 customers located across the US, each of which has demand for five different glass products. The glass products are made at four different US plants. Currently, the company produces each product at one location only and serves each customer directly from the source plant.
The manufacturer is experiencing two major problems at the moment:
i) service to some distant customers has been unreliable and
ii) rising gas prices have had a large impact on the balance sheet through transportation costs.
The manufacturer wants to explore 2 options (either individually or in tandem) to improve the service and decrease transportation costs:
i) build warehouses ii) upgrade plants
Opex Analytics - Consulting Solutions
The consulting team at Opex Analytics has been tasked with building a model to help the CEO determine if either of these two changes should be made. In order to do this, we will need to use the model to determine how the proposed changes to the supply chain would affect performance relative to the current state.
Mathematical Modeling
The mathematical model is defined as a mixed-integer programming problem. The 2 options - building of warehouses and upgradation of plants - are analysed individually as well as in tandem.

 In all, a total of 4 configurations are analysed whose results and codes are available in the .zip file:
   Configuration A Configuration B Configuration C Configuration D
Current state of the SC
Only warehouses are built
Only the plants are upgraded
Warehouses are built and plants are upgraded
Recommended Solution
Sub-optimal Configurations
                  About the programming aspect of the model:
i) The model is built using the Pulp library in Python 3.5.
ii) CBC solver is used to find the solutions.
iii) All the codes are run on Macbook Pro 2.3 GHz Intel Core i5, and do not take more than 10 mins to produce the results and write the solution to excel files.
The results in brief, for the 4 configurations are as follows:
Conf.A 143 98 11 0 Conf.B 135 108 80 6 Conf.C 187 54 43 0 Conf.D 181 59 80 3
  Profit (Million USD)
  Transportation Cost (Million USD)
   Service %
   No. of warehouses
                                      
 Opex_Case_Study_Sol.zip The .zip file contains 4 folders:
1. Read Me
It contains 4 files:
i) Case Study - Problem Statement.pdf
It contains the complete description of the problem statement, objectives and deliverables.
ii) Opex Case Study Write-up.pdf The current file.
iii) Code Run.pdf
Contains information on changes to be made to run the code.
iv) 1316_Network_Planning.xlsx
The file which contains data supplied to the optimisation model.
2. Presentation
It contains one .pdf file - ​“Opex Case Study PPT - Ankit, 25_10_2020.pdf” to be delivered before the CEO, senior-management and technical experts.
3. Codes
It contains 4 Jupyter Notebooks.
i) Conf. A - Current SC.ipynb
It contains the profit/cost analysis of the SC in the current state.
ii) Conf. B - Only_Warehouses.ipynb
It contains the profit/cost analysis when only warehouses are built in the SC.
iii) Conf. C - Only_Plant_upgrades.ipynb
It contains the profit/cost analysis when only the plants are upgraded.

 iv) Conf. D - Plant_Upgrade_and_Warehouses.ipynb
It contains the profit/cost analysis when plants are upgraded and warehouses are built in the SC.
Each notebook has the following results printed in it:
i) No. of warehouses to be built and their locations
ii) Product assignments - which product are produced at which plant and in what quantities. iii) Total cost, revenue, profits
iv) Break-up of total cost into transportation, changeover and production cost
v) Breakup of transportation cost into Plant → Customer, Plant → Warehouse and Warehouse → Customer shipping cost.
vi) Service % (*Service = % of total demand met by a facility within 500 mi of the customer ) vii) Upgradation decision for each plant
viii) Changeover (set-up) decisions between the products at each plant
4. Result Files
It contains 4 excel files, each corresponding to one of the 4 configurations.
Each excel file contains the following sheets:
i) Balance Sheet
It contains the overall values for costs, revenues and profits.
ii) Total costs Breakup
It contains the break-up of total cost into transportation cost, changeover cost and production cost.
iii) Transportation Costs Breakup
It breaks up the transportation cost into 3 components:
Plant → Customer, Plant → Warehouse and Warehouse → Customer shipping cost

 iv) Product Assignments
It identifies which product is produced at which plant.
v) Production Quantities
It gives the quantity of a product produced at a given plant.
vi) Qty - Plants to Warehouse
vii) Qty - Plants to Customer
viii) Qty - Warehouse to Customer
These 3 sheets identify the quantities of each product transported from Plants → Warehouses, Plants → Customers and Warehouses → Customers respectively.
