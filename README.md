# D3 Homework - Data Journalism and D3

## Purpose
* The purpose of this assignment was to use the data set from the US Census to investigate rates of income, obesity, poverty, etc. by state to build a scatterplot
* The dataset: https://data.census.gov/cedsci/

## Key Skills
* JavaScript
* D3.js
* D3.js interactive visualization
* tooltips

### Step 1 - Create a Skeleton
* Before attempting to plot, I first load in the CSV and did a `console.log` to make sure I correctly loaded the CSV
* Next, I made sure that my margins were appropriate so that I can properly do a scatterplot
* This assignment had two parts - main assignment and bonus assignment. I first did the main assignment to make sure that I could get the most basic scatter plot.

### Step 2 - Plot basic scatterplot
* The main assigment required to create a scatter plot between two of the data variables such as `Healthcare vs. Poverty` or `Smokers vs. Age`.
* Once the scatter plot was created, I added a state abbreviations to each circle. 
```
 var circleText = chartGroup.selectAll()
    .data(data)
    .enter()
    .append("text")
    .text(d => d.abbr)
    .attr("x", d => xLinearScale(d[xProperty])) 
    .attr("y", d => yLinearScale(d[yProperty])) 
    .attr("class", "stateText") 
    .attr("font-size", "9");
```
### Step 3 - Bonus
* The bonus portion required additional variables and tooltip with interactions.

