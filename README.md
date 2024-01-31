# Optimizing-Supply-Chain-Strategies
Optimizing Supply Chain Strategies for Tech Haven: Navigating Unit Costs and Demand Uncertainties in the Smartphone Retail Landscape

![image](https://github.com/Lawrence-le/Optimizing-Supply-Chain-Strategies/assets/151991077/62b649a4-52e6-48e4-a520-226685b09553)

# Background
Tech Haven, a leading technology retailer with numerous locations across the nation, faces the challenge of efficiently ordering the latest gadgets and distributing them to its individual stores. 

# Scenario
In this case, let's consider a popular new smartphone model, which Tech Haven plans to sell for $800. The unit cost for each device depends on the quantity ordered, and Tech Haven wants to optimize its ordering strategy.

For the smartphone model:

If the number ordered is less than 1000, the unit cost is $700.
After each 1000 units, the unit cost drops:
$690 for at least 1000 units
$680 for at least 2000 units
$670 for at least 3000 units
$660 (the lowest possible unit cost) for at least 4000 units.

Tech Haven faces uncertainty about the demand for this smartphone, estimating that it could range from 500 to 5000 units. Additionally, considering the fast-paced nature of the technology industry, Tech Haven recognizes that newer models will be released, potentially affecting the demand for this specific smartphone.

If there are any unsold smartphones when the next model is released, Tech Haven plans to reduce the price to $500, believing that at this discounted price, all remaining devices will be sold.

# Objectives
Find the optimized ordering strategy using data visualisation.

## Create a table using excel to find out the following
* Surplus
* Cost
* Revenue
* Profit

![image](https://github.com/Lawrence-le/Optimizing-Supply-Chain-Strategies/assets/151991077/47676847-677c-4978-8fbf-b5d95b7e90dd)

For Surplus there are 2 types of method used
1. MAX() this method compare demand and order and output the max between the two. If the value is negative, the value is replaced with 0
2. IF() : If Order is more than Supply, cell output Order-Demand, else the output will be 0

For Cost we need to create a Data Table

![image](https://github.com/Lawrence-le/Optimizing-Supply-Chain-Strategies/assets/151991077/6ea6d913-aac1-40f6-88c2-f0c0b3822c35)


VLOOKUP() is used to find the lookup the value that corresponds to the number of orders that matches with the unit price in the data table

For Revenue, is computed by:
MIN(of demand vs order) x Regular Price + Sale Price x  Surplus

Finally Profit is computed by:
Revenue - Cost

To find the optimized order number to maximise proft we need to create a table to show the Order vs Demand.  
In order to achieve the tabulated table, we need to use Excel Feature What-If Analysis's Data Table.

![image](https://github.com/Lawrence-le/Optimizing-Supply-Chain-Strategies/assets/151991077/29b9212f-6015-4c1c-8bd0-1b14345e9e65)

# Conclusion:

From the colour coded table, red represents the lowest profit and green represents the highest profit.  
In order to achieve the optimized order to achieve profitability, we need to ensure that order has to be lower than demand for minimal risk.

## The optimization of supply chain strategies for Tech Haven, as outlined in the scenario, offers several potential benefits:

Cost Efficiency: By optimizing the ordering strategy based on quantity, Tech Haven can minimize the unit cost of each smartphone. This cost efficiency becomes particularly significant as the order quantity increases, allowing the company to maximize profit margins.

Inventory Management: Efficient ordering strategies help Tech Haven manage its inventory effectively. By aligning orders with anticipated demand and adjusting unit costs accordingly, the company can avoid overstocking or understocking issues.

Competitive Pricing: The ability to offer smartphones at competitive prices enhances Tech Haven's competitiveness in the market. Lower unit costs allow the company to set competitive retail prices, attracting more customers and potentially increasing market share.

Adaptability to Market Changes: Considering the fast-paced nature of the technology industry, Tech Haven's ability to adjust its ordering strategy based on market dynamics and new product releases ensures adaptability. This flexibility helps in mitigating risks associated with changes in consumer preferences and technological advancements.

Minimizing Losses on Obsolete Inventory: The strategy of reducing the price to $500 for unsold smartphones when a new model is released helps minimize losses on obsolete inventory. This approach aligns with market realities, allowing Tech Haven to clear out older stock efficiently.

Customer Satisfaction: Offering smartphones at competitive prices and promptly introducing discounts for older models can enhance customer satisfaction. Customers may be more inclined to make purchases from Tech Haven, knowing that the company is responsive to market trends and provides value for money.

## Summary
The optimization of supply chain strategies benefits Tech Haven by improving cost efficiency, inventory management, market competitiveness, adaptability to industry changes, and overall customer satisfaction.




