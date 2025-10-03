# Uber Rides Data Analysis

## Project Overview
This project analyzes Uber rides data to provide insights into customer booking behavior. The dataset contains **1156 rows and 7 columns**, with some missing values. The analysis focuses on ride categories, purposes, booking times, frequency, and travel distances.

## Dataset Description
Columns in the dataset:
- `START_DATE` – Date and time when the ride started
- `END_DATE` – Date and time when the ride ended
- `CATEGORY` – Type of ride (e.g., Business, Personal)
- `START` – Pickup location
- `STOP` – Drop location
- `MILES` – Distance of the ride in miles
- `PURPOSE` – Reason for the ride (e.g., Meeting, Meal, Not Specified)

## Data Cleaning & Preparation
1. Filled missing values in the `PURPOSE` column with `"Not Available"`.
2. Dropped rows with other null values.
3. Converted `START_DATE` and `END_DATE` to `datetime` format.
4. Created new columns for:
   - `Month`
   - `Day of Week`
   - `Hour`
5. Grouped `Hour` into time periods:
   - Morning
   - Afternoon
   - Evening
   - Night
6. Removed duplicate rows.
7. Saved the cleaned dataset for analysis.

## Data Analysis & Visualization

### 1. Most Booked Category
- **Insight:** Business rides are booked more frequently than Personal rides.  
- **Visualization:**
![Most Booked Category and purpose](images1/subplots.png)

### 2. Purpose of Rides
- **Insight:** Most people do not specify a purpose. Among specified purposes, **Meal/Entertainment** and **Meeting** purposes are the most common.  

### 3. Peak Booking Time
- **Insight:** Rides are most frequently booked in the **Morning** and **Evening**.  
- **Visualization:**
![Peak Booking Time](images1/time_vs_cabs.png)