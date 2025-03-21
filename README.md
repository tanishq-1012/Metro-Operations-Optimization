# Metro-Operations-Optimization

## Overview

Metro Operations Optimization refers to the systematic process of enhancing the efficiency, reliability, and effectiveness of Metro services through various data-driven techniques and operational adjustments.
This project focuses on optimizing the operations of the Delhi Metro using Python. It utilizes General Transit Feed Specification (GTFS) data to analyze metro routes, stop locations, trip schedules, and frequency distributions. The project provides insights into metro coverage, trip distributions, stop density, and optimized scheduling based on time-of-day demand.

## Features

**GTFS Data Processing**: Load and analyze various GTFS datasets such as routes, trips, stops, and stop_times.

**Geographical Visualization**:

Plot Delhi Metro routes on a map.

Visualize metro stop locations.

Highlight the number of routes passing through each stop.

**Trip Analysis**:

Count and visualize the number of trips per day of the week.

Analyze the time intervals between metro trips at different stops.

Categorize trips into different time intervals (Morning Peak, Midday, Evening Peak, etc.).

**Schedule Optimization**:

Adjust trip frequencies based on demand during peak and off-peak hours.

Compare original vs. optimized schedules for efficiency improvements.

## Dataset

The dataset contains several files as follows:

1.**Agency**: Information about the Delhi Metro Rail Corporation, including name, URL, and contact details.

2.**Calendar**: Service schedules delineating the operation days (weekdays, weekends) and valid dates for these schedules.

3.**Routes**: Details of metro routes, including short and long names, type of route, and descriptions.

4.**Shapes**: Geographical coordinates of routes, providing the precise paths taken by the metro lines.

5.**Stop Times**: Timetables for each trip indicating arrival and departure times at specific stops.

6.**Stops**: Locations of metro stops, including latitude and longitude coordinates.

7.**Trips**: Information linking trips to routes, including details like trip identifiers and associated route IDs.

<img width="810" alt="Screenshot 2025-03-21 at 3 08 57 PM" src="https://github.com/user-attachments/assets/2ea5e85f-f180-469c-b391-4c389f975a8e" />

<img width="810" alt="Screenshot 2025-03-21 at 3 09 32 PM" src="https://github.com/user-attachments/assets/160ba775-f96c-403d-99af-4f8e8d26572e" />

<img width="810" alt="Screenshot 2025-03-21 at 3 10 24 PM" src="https://github.com/user-attachments/assets/bf6630e1-86a7-40bf-b0b1-8e7fcc39ad7d" />

## Plot 1

Let's start by analyzing the routes and operations of Delhi Metro to understand how it operates. We'll start by:

1. Plotting the geographical routes on map to visualize the network.

2. Examining the frequency and scheduling of trips across different days of the week.

3. Analyzing coverage by examining the distribution of stops and their connectivity.

I’ll start by plotting the geographical paths of different routes on a map to visualize how the Delhi Metro covers the area:

<img width="656" alt="Screenshot 2025-03-21 at 3 10 50 PM" src="https://github.com/user-attachments/assets/cf1e4c2d-0529-43b1-a83b-f55a4185d002" />

The map visualization shows the geographical paths of the Delhi Metro routes. Each line (identified by a unique colour) represents the path of a different route defined in the shapes dataset. This visual helps to understand how the Metro covers the geographical area of Delhi, demonstrating the connectivity and spread of the network.

## Plot 2

Next, I will examine the frequency and scheduling of trips across different days of the week by analyzing the calendar and trip data:

<img width="656" alt="Screenshot 2025-03-21 at 3 11 11 PM" src="https://github.com/user-attachments/assets/c8e08be6-9387-4ec3-a40a-800fd9c3ce8e" />

The bar chart illustrates the number of trips scheduled for each day of the week for the Delhi Metro. As we can see, the number of trips from Monday to Friday is consistent, indicating a stable weekday schedule designed to accommodate regular commuter traffic. In contrast, the trips decrease slightly on Saturday and even more on Sunday, reflecting lower demand or a reduced service schedule on weekends.

This finding suggests that the Delhi Metro strategically scales its operations based on the expected daily ridership, which likely peaks during weekdays due to work and school commutes.

## Plot 3

To further analyze the connectivity and effectiveness of the route strategy, I will analyze the distribution and connectivity of stops:

<img width="656" alt="Screenshot 2025-03-21 at 3 11 36 PM" src="https://github.com/user-attachments/assets/ca6c75c0-4f5b-4d4f-8637-2ec9eae90b44" />

The scatter plot above shows the geographical distribution of Delhi Metro stops. Each red dot represents a metro stop, and their distribution across the map illustrates how the stops cover different areas of Delhi.

From the plot, we can see a widespread distribution, suggesting that the Delhi Metro provides good spatial coverage, allowing access to a broad area and facilitating efficient travel across the city.

The stops are fairly evenly spread, but there are denser clusters, which indicates areas with higher transit needs or central hubs that connect multiple lines.

## Plot 4

Now, let’s analyze the route complexity. I will analyze how many routes pass through each stop, which can highlight key transfer points and central hubs within the Delhi Metro network:

<img width="656" alt="Screenshot 2025-03-21 at 3 12 08 PM" src="https://github.com/user-attachments/assets/47770690-e53f-4b95-ba95-d543348a426a" />

The scatter plot above represents the number of routes that pass through each Delhi Metro stop. Stops are visualized in different colours and sizes based on the number of routes they connect, providing insights into the complexity of the network at various locations. Key observations are:

**Hubs and Transfer Points**: Larger circles (in warmer colours) indicate stops where multiple routes intersect. These stops serve as major transfer points within the network, facilitating easier cross-city travel for passengers.

**Distribution**: Stops with fewer routes, shown in cooler colours and smaller sizes, tend to be more peripheral or on less busy lines. The central areas and more populated zones have stops with greater connectivity.

## Plot 5

Next, let’s analyze the service frequency by examining the timing intervals between trips during different parts of the day. It will help us understand peak and off-peak operational strategies, which are crucial for managing commuter flow efficiently. Let’s calculate and visualize these intervals:

<img width="555" alt="Screenshot 2025-03-21 at 3 12 40 PM" src="https://github.com/user-attachments/assets/61362a12-79fa-4ed6-b04b-221e1f9d45e2" />

The bar chart above displays the average interval between trips on the Delhi Metro during different parts of the day: morning, afternoon, and evening. This data provides insight into the service frequency and how it is adjusted based on the expected demand throughout the day. Key findings are:

**Morning**: Shorter intervals between trips are observed in the morning hours, which likely corresponds to the morning rush hour when commuters are heading to work or school.

**Afternoon**: The intervals increase slightly during the afternoon, which may indicate a reduction in demand after the morning peak.

**Evening**: In the evening, intervals decrease again, likely to accommodate the evening rush hour as people return home.











