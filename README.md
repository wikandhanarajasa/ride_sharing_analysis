# Chicago Ride-Sharing Analysis

## Introduction

This project aims to understand the pattern of ride-sharing activities in the city of Chicago, helping Zuber successfully penetrate this particular area.

## Goal

The objectives of this project are outlined below.

- Understanding the habits of passengers during certain weather conditions and destinations.
- Identifying the top 10 destinations of ride-sharing services.
- Identifying the top 10 taxi companies in the Chicago area.
- Testing hypotheses related to ride-sharing patterns.

## Stages

The project's phases are outlined below.

1. **Open the data file and study its general information.**

2. **Prepare the data.**
   - Rename the columns (use lowercase letters for all).
   - Convert the data to the required data type.
   - Describe which columns have had their data types changed and explain the reasons.
   - Handle missing values if necessary.
   - Calculate the total sales (sales quantity across all regions) for each game and input these values into a separate column.

3. **Analyze the data.**
   - Using Python, identify the top 10 destinations.
   - Sort the table to get the top 10 destinations in Chicago.
   - Sort the top taxi companies' performance.
   - Create graphs to help visualize the data.
   - Summarize the main findings.

4. **Test hypotheses.**
   - Test the hypothesis that trips to O'Hare from Loop change during bad weather.
   - Set the hypotheses:
     - H0: The average trip from Loop to O'Hare airport during rain on Saturday is the same.
     - H1: The average trip from Loop to O'Hare airport during rain on Saturday is different.
   - Set the alpha level (0.05).
   - Draw the final conclusion.

## Data Description

The dataset includes the following tables and columns:

### Neighborhoods Table
- **name:** Neighborhood name
- **neighborhood_id:** Neighborhood code

### Cabs Table
- **cab_id:** Vehicle code
- **vehicle_id:** Technical vehicle ID
- **company_name:** Name of the company that owns the vehicle

### Trips Table
- **trip_id:** Trip code
- **cab_id:** Operating vehicle code
- **start_ts:** Date and time trip started (time rounded to the nearest hour)
- **end_ts:** Date and time trip ended (time rounded to the nearest hour)
- **duration_seconds:** Trip duration in seconds
- **distance_miles:** Trip distance in miles
- **pickup_location_id:** Pickup location code
- **dropoff_location_id:** Drop-off location code

### Weather Records Table
- **record_id:** Weather recording code
- **ts:** Date and time when weather recording was done (time rounded to the nearest hour)
- **temperature:** Temperature at the time of weather recording
- **description:** Brief description of weather conditions, such as "light rain" or "scattered clouds."

## Conclusion

This project aims to understand the pattern of ride-sharing activities in the city of Chicago, helping Zuber successfully penetrate this particular area.

### Data Initiation

#### Taxi
- **company_name:** Name of taxi companies
- **trips_amount:** Number of trips of each taxi company

#### Trips
- **dropoff_location_name:** Destination of trip
- **average_trips:** Number of trips

#### Trip_Ohare
- **start_ts:** Date of trip
- **weather_conditions:** Condition of weather
- **duration_seconds:** Duration of trip

### Data Analyzing

**Findings:**
- The top 3 destinations are Loop, River North, & Streeterville.
- The top 3 taxi companies in the Chicago area are Flash Cab, Taxi Affiliation Service, & Medallion Leasing.

**Insights:**
- The top 4 destinations make up the majority of destinations in the Chicago area.
- Flash Cab dominates the competition in the Chicago area.

**Recommendations:**
- Zuber should prioritize hiring driver partners from the top 4 areas to boost their efficiency and take advantage of trip patterns.
- Learn from Flash Cab's success and set the price slightly below Flash Cab in the top 4 areas.

### Hypothesis Testing

Based on the hypothesis testing:

**Using Levene Method:**
- **p-value:** 0.3563611473946102
- H0 is accepted: The average trip from Loop to O'Hare airport during rain and not rain on Saturday is the same.
- The average trip from Loop to O'Hare during good weather on Saturday is 1976.8163265306123 seconds.
- The average trip from Loop to O'Hare during bad weather on Saturday is 2434.785310734463 seconds.

**Using T-test:**
- **p-value:** 9.108025319217097e-15
- H0 is rejected: The average trip from Loop to O'Hare airport during rain and not rain on Saturday is different.
- The average trip from Loop to O'Hare during good weather on Saturday is 1976.8163265306123 seconds.
- The average trip from Loop to O'Hare during bad weather on Saturday is 2434.785310734463 seconds.

**Highlights:**
- The top 3 destinations are Loop, River North, & Streeterville, all located in downtown Chicago.
- Flash Cab is the most popular company based on trips.
- There is a significant increase in service demand during bad weather from downtown to the airport.

**Recommendations:**
- Zuber needs to focus on selling its product to urban areas or 9-5 workers mostly located downtown.
- Benchmarking should be done against Flash Cab, Taxi Affiliation Service, & Medallion Leasing.
- For high-demand areas like downtown, Zuber should offer competitive pricing to attract initial customers.
- For a city with four seasons and a car culture like Chicago, weather significantly affects ride-sharing services. A strategy for fluctuating prices based on demand should be implemented to gain revenue.
