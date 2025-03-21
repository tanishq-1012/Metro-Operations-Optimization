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






