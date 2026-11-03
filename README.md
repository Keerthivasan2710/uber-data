# Uber Ride Booking Analysis Dashboard

## Project Overview
This project analyzes NCR Uber ride-booking data to understand booking performance, ride completion, cancellations, vehicle usage, revenue, and customer/driver ratings. The dashboard is designed in Microsoft Power BI.

## Dataset
- **File:** `ncr_ride_bookings.csv`
- **Records:** 150,000
- **Columns:** 21
- **Date coverage:** 2024 (based on the dataset's Date field)

### Important fields
- Booking Date and Time
- Booking Status
- Vehicle Type
- Pickup Location and Drop Location
- Booking Value and Ride Distance
- Average VTAT and Average CTAT
- Driver Ratings and Customer Rating
- Payment Method
- Customer and Driver Cancellation Reasons
- Incomplete Ride Reasons

## Dashboard Goals
1. Track total bookings and completed bookings.
2. Measure booking completion and cancellation rates.
3. Compare bookings by vehicle type and payment method.
4. Identify popular pickup and drop locations.
5. Analyze booking value and ride distance.
6. Understand customer and driver ratings.
7. Explore reasons for cancellations and incomplete rides.

## Suggested Dashboard Pages

### 1. Overview
- Total Bookings
- Completed Bookings
- Cancelled Bookings
- Incomplete Bookings
- Completion Rate
- Total Booking Value
- Bookings by month
- Booking status breakdown

### 2. Vehicle and Location Analysis
- Bookings by vehicle type
- Booking value by vehicle type
- Top pickup locations
- Top drop locations
- Ride distance by vehicle type

### 3. Cancellation and Incomplete Ride Analysis
- Customer cancellations
- Driver cancellations
- No-driver-found bookings
- Cancellation reasons
- Incomplete ride reasons

### 4. Customer and Payment Analysis
- Customer ratings
- Driver ratings
- Payment method distribution
- Booking value by payment method

## Tools Used
- Microsoft Power BI Desktop
- Power Query for data cleaning and transformation
- DAX for calculated measures
- Git and GitHub for version control and project sharing

## How to Open the Project
1. Download or clone this repository.
2. Open `Uber.pbix` using Microsoft Power BI Desktop.
3. If necessary, update the CSV source path in Power BI using **Transform data** or **Data source settings**.
4. Apply changes and refresh the report.

## How to Rebuild the Dashboard
1. Open Power BI Desktop.
2. Select **Get data → Text/CSV**.
3. Select `ncr_ride_bookings.csv`.
4. Choose **Transform Data** to inspect data types, blanks, and inconsistent values.
5. Select **Close & Apply**.
6. Create DAX measures for booking KPIs.
7. Add cards, bar charts, line charts, donut charts, and slicers.
8. Save the report as `Uber.pbix`.

## Suggested GitHub Repository Structure

```text
uber-ride-booking-analysis/
├── data/
│   └── ncr_ride_bookings.csv
├── dashboard/
│   └── Uber.pbix
├── images/
│   └── dashboard-preview.gif
├── README.md
└── .gitignore
```

## Data Notes
- The dataset contains missing values in several fields. For example, ratings, payment methods, booking values, and ride distances are not populated for every booking. Check the meaning of each missing value before replacing or deleting it.
- Do not automatically treat every blank as zero.
- Define the denominator used for each KPI clearly. For example, calculate average ratings only from records with a rating.
- Confirm the date range and currency/unit definitions from the dataset documentation, if available.

## Future Improvements
- Add date, vehicle type, booking status, and payment method slicers.
- Add drill-through pages for locations and cancellation reasons.
- Improve report layout, tooltips, and mobile view.
- Add a dashboard screenshot or GIF to the repository.

## Author
**Keerthivasan P**

## License
Add a license only if you have permission to share the dataset and dashboard files publicly. Check the dataset's source and usage terms before uploading the CSV to GitHub.
