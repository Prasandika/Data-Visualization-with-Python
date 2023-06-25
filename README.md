# Data-Visualization-with-Python
## Story:
As a data analyst, you have been given a task to monitor and report US domestic airline flights performance. Goal is to analyze the performance of the reporting airline to improve fight reliability thereby improving customer relaibility.

Below are the key report items,

Yearly airline performance report
Yearly average flight delay statistics
NOTE: Year range is between 2005 and 2020.

## Components of the report items
1. Yearly airline performance report

For the chosen year provide,

Number of flights under different cancellation categories using bar chart.
Average flight time by reporting airline using line chart.
Percentage of diverted airport landings per reporting airline using pie chart.
Number of flights flying from each state using choropleth map.
Number of flights flying to each state from each reporting airline using treemap chart.
Yearly average flight delay statistics

2. For the chosen year provide,

Monthly average carrier delay by reporting airline for the given year.
Monthly average weather delay by reporting airline for the given year.
Monthly average natioanl air system delay by reporting airline for the given year.
Monthly average security delay by reporting airline for the given year.
Monthly average late aircraft delay by reporting airline for the given year.
NOTE: You have worked created the same dashboard components in Flight Delay Time Statistics Dashboard section. We will be reusing the same.

## Requirements to create the dashboard
Create dropdown using the reference here
Create two HTML divisions that can accomodate two components (in one division) side by side. One is HTML heading and the other one is dropdown.
Add graph components.
Callback function to compute data, create graph and return to the layout.

## What's new in this exercise compared to other labs?
Make sure the layout is clean without any defualt graphs or graph layouts. We will do this by 3 changes:

1. Add app.config.suppress_callback_exceptions = True right after app = JupyterDash(__name__).
2. Having empty html.Div and use the callback to Output the dcc.graph as the Children of that Div.
3. Add a state variable in addition to callback decorator input and output parameter. This will allow us to pass extra values without firing the callbacks. Here, # we need to pass two inputs chart type and year. Input is read only after user entering all the information.
Use new html display style flex to arrange the dropdown menu with description.

Update app run step to avoid getting error message before initiating callback.

NOTE: These steps are only for review.

## Review
Search/Look for review to know how commands are used and computations are carried out. There are 7 review items.

1. REVIEW1: Clear the layout and do not display exception till callback gets executed.
2. REVIEW2: Dropdown creation.
3. REVIEW3: Observe how we add an empty division and providing an id that will be updated during callback.
4. REVIEW4: Holding output state till user enters all the form information. In this case, it will be chart type and year.
5. REVIEW5: Number of flights flying from each state using choropleth
6. REVIEW6: Return dcc.Graph component to the empty division
7. REVIEW7: This covers chart type 2 and we have completed this exercise under Flight Delay Time Statistics Dashboard section
