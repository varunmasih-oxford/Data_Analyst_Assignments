# Project 7: Hotel & Hospitality Analytics

## 1. Business Scenario

Hotel management wants to improve occupancy, room revenue, guest satisfaction and booking-channel efficiency across its properties.

Your task is to act as a **Business Data Analyst** and convert the raw operational data into a Pivot Table-based management report.

---

## 2. Dataset Overview

This project is designed to practice:

- Excel Tables
- Pivot Tables
- Pivot Charts
- Slicers
- Timeline
- KPI calculations
- Benchmark comparison
- Conditional Formatting
- Business insights
- Management decision-making

### Dataset Columns

| Column | Description |
|---|---|
| Booking_ID | Booking identifier |
| Month | Booking month |
| Hotel | Hotel property |
| City | City |
| Room_Type | Room category |
| Booking_Channel | Booking source |
| Customer_Type | Customer segment |
| Nights | Number of nights |
| Room_Rate | Average nightly room rate |
| Room_Revenue | Room revenue |
| Cancelled | Yes/No |
| Occupancy_% | Occupancy percentage |
| Guest_Rating | Guest rating out of 5 |
| Complaints | Number of complaints |
| Checkin_Delay_Min | Check-in delay in minutes |

---

## 3. Dataset

Save the following data as:

`07_hotel_hospitality_analytics.csv`

```csv
Booking_ID,Month,Hotel,City,Room_Type,Booking_Channel,Customer_Type,Nights,Room_Rate,Room_Revenue,Cancelled,Occupancy_%,Guest_Rating,Complaints,Checkin_Delay_Min
BKG001,2026-01,Hotel South,Bangalore,Suite,Direct,Family,5,10767,53835,No,70.0,4.4,0,24
BKG002,2026-02,Hotel Central,Jaipur,Standard,Corporate,Leisure,1,13345,13345,Yes,89.3,3.5,0,26
BKG003,2026-03,Hotel North,Bangalore,Suite,OTA,Leisure,6,5008,30048,No,83.1,3.4,3,42
BKG004,2026-04,Hotel North,Mumbai,Deluxe,OTA,Leisure,7,4218,29526,No,80.3,3.8,0,31
BKG005,2026-05,Hotel Central,Bangalore,Standard,Direct,Business,6,9213,55278,No,56.6,4.1,1,44
BKG006,2026-06,Hotel South,Delhi,Suite,Direct,Leisure,6,3958,23748,No,89.2,4.4,1,5
BKG007,2026-01,Hotel North,Delhi,Deluxe,Corporate,Family,6,6287,37722,No,95.1,3.8,0,6
BKG008,2026-02,Hotel North,Mumbai,Deluxe,Corporate,Leisure,3,9479,28437,No,58.9,4.5,0,0
BKG009,2026-03,Hotel Central,Jaipur,Deluxe,Corporate,Leisure,5,6895,34475,No,58.8,4.6,1,7
BKG010,2026-04,Hotel South,Delhi,Standard,Direct,Leisure,6,10335,62010,No,81.6,4.6,0,8
BKG011,2026-05,Hotel South,Delhi,Suite,OTA,Leisure,5,10408,52040,No,82.8,3.7,3,22
BKG012,2026-06,Hotel South,Mumbai,Suite,Corporate,Family,4,4350,17400,No,73.1,3.5,2,0
BKG013,2026-01,Hotel Central,Jaipur,Standard,Direct,Business,5,13776,68880,No,58.9,4.4,1,30
BKG014,2026-02,Hotel Central,Bangalore,Standard,Corporate,Leisure,6,5071,30426,No,74.2,4.1,1,4
BKG015,2026-03,Hotel Central,Jaipur,Suite,Travel Agent,Business,1,10805,10805,No,81.4,4.0,1,5
BKG016,2026-04,Hotel Central,Jaipur,Standard,Direct,Business,7,10666,74662,No,59.9,4.1,0,6
BKG017,2026-05,Hotel South,Jaipur,Deluxe,Corporate,Business,7,12399,86793,No,81.1,4.7,4,13
BKG018,2026-06,Hotel South,Bangalore,Suite,Travel Agent,Business,7,6152,43064,No,68.6,4.6,4,30
BKG019,2026-01,Hotel South,Bangalore,Suite,Direct,Business,1,14940,14940,No,55.1,3.9,2,35
BKG020,2026-02,Hotel South,Mumbai,Standard,Direct,Leisure,2,10567,21134,No,84.4,4.5,0,16
BKG021,2026-03,Hotel South,Delhi,Deluxe,Travel Agent,Family,2,9988,19976,No,62.8,3.9,3,2
BKG022,2026-04,Hotel Central,Jaipur,Suite,OTA,Family,5,10760,53800,No,75.5,4.2,0,35
BKG023,2026-05,Hotel Central,Jaipur,Deluxe,OTA,Leisure,5,5345,26725,No,60.3,4.0,4,38
BKG024,2026-06,Hotel South,Bangalore,Suite,Corporate,Family,4,8117,32468,No,73.6,3.6,3,38
BKG025,2026-01,Hotel Central,Mumbai,Suite,OTA,Family,6,11569,69414,No,63.2,4.3,2,43
BKG026,2026-02,Hotel South,Jaipur,Suite,Corporate,Leisure,5,13875,69375,No,84.1,4.5,4,30
BKG027,2026-03,Hotel Central,Mumbai,Deluxe,Corporate,Business,7,2709,18963,No,56.0,3.6,0,12
BKG028,2026-04,Hotel Central,Delhi,Suite,OTA,Family,7,3516,24612,No,67.1,4.5,0,22
BKG029,2026-05,Hotel South,Delhi,Deluxe,Travel Agent,Leisure,6,11695,70170,No,75.9,4.6,2,44
BKG030,2026-06,Hotel South,Jaipur,Standard,Corporate,Family,7,13725,96075,No,77.6,3.4,2,12
BKG031,2026-01,Hotel North,Delhi,Standard,OTA,Family,5,14598,72990,No,86.8,4.8,2,28
BKG032,2026-02,Hotel South,Bangalore,Standard,Corporate,Leisure,5,4455,22275,No,72.6,4.2,1,10
BKG033,2026-03,Hotel Central,Jaipur,Suite,Corporate,Business,6,5036,30216,Yes,93.1,4.3,4,42
BKG034,2026-04,Hotel North,Jaipur,Suite,Travel Agent,Business,7,14094,98658,No,64.0,3.7,0,32
BKG035,2026-05,Hotel South,Jaipur,Suite,Direct,Business,3,6124,18372,No,82.2,3.9,2,13
BKG036,2026-06,Hotel North,Bangalore,Deluxe,Direct,Leisure,6,8168,49008,No,92.1,4.3,4,15
BKG037,2026-01,Hotel South,Jaipur,Deluxe,Direct,Leisure,3,11351,34053,No,56.0,4.2,2,32
BKG038,2026-02,Hotel North,Delhi,Standard,OTA,Family,6,5654,33924,No,58.4,3.5,4,34
BKG039,2026-03,Hotel North,Mumbai,Standard,Travel Agent,Family,4,4202,16808,No,89.0,4.7,3,41
BKG040,2026-04,Hotel South,Mumbai,Deluxe,Travel Agent,Leisure,3,3120,9360,Yes,57.2,4.6,4,4
BKG041,2026-05,Hotel North,Delhi,Suite,Direct,Family,4,12825,51300,No,68.0,4.0,0,34
BKG042,2026-06,Hotel North,Bangalore,Deluxe,Travel Agent,Leisure,7,3689,25823,No,75.6,3.8,2,38
BKG043,2026-01,Hotel Central,Mumbai,Deluxe,Corporate,Business,7,13325,93275,Yes,61.4,3.7,3,34
BKG044,2026-02,Hotel South,Delhi,Deluxe,OTA,Family,5,11594,57970,No,56.7,4.3,3,34
BKG045,2026-03,Hotel North,Mumbai,Standard,Corporate,Business,6,14393,86358,No,71.9,4.4,4,9
BKG046,2026-04,Hotel South,Delhi,Deluxe,Direct,Leisure,1,5471,5471,No,78.3,3.5,4,29
BKG047,2026-05,Hotel South,Mumbai,Standard,Corporate,Family,1,5734,5734,No,75.0,3.9,1,42
BKG048,2026-06,Hotel South,Mumbai,Suite,Corporate,Leisure,1,5670,5670,No,73.5,4.3,2,44
BKG049,2026-01,Hotel Central,Mumbai,Suite,Corporate,Leisure,4,5262,21048,Yes,65.1,3.7,3,17
BKG050,2026-02,Hotel South,Delhi,Deluxe,OTA,Family,4,9796,39184,No,67.5,4.2,1,41
BKG051,2026-03,Hotel South,Delhi,Suite,Travel Agent,Family,2,6812,13624,No,80.7,4.5,0,32
BKG052,2026-04,Hotel North,Bangalore,Deluxe,OTA,Family,2,3100,6200,No,77.3,4.9,3,41
BKG053,2026-05,Hotel North,Mumbai,Suite,OTA,Family,6,7267,43602,No,75.5,3.5,2,32
BKG054,2026-06,Hotel Central,Delhi,Standard,Travel Agent,Business,2,9810,19620,No,78.2,4.2,1,30
BKG055,2026-01,Hotel Central,Jaipur,Standard,Direct,Family,1,6831,6831,No,56.8,3.7,2,24
BKG056,2026-02,Hotel South,Mumbai,Deluxe,Travel Agent,Leisure,3,4191,12573,No,76.4,4.6,2,37
BKG057,2026-03,Hotel Central,Bangalore,Deluxe,Travel Agent,Leisure,5,13204,66020,No,58.2,3.8,1,33
BKG058,2026-04,Hotel South,Bangalore,Standard,OTA,Business,5,2608,13040,No,60.7,3.6,0,32
BKG059,2026-05,Hotel South,Delhi,Deluxe,Travel Agent,Leisure,2,8434,16868,No,88.5,4.4,3,21
BKG060,2026-06,Hotel South,Mumbai,Standard,Direct,Family,2,12179,24358,No,89.2,3.4,0,8
```

---

## 4. Business / Industry Benchmarks

Use these benchmark values for the analysis.

| KPI | Benchmark |
|---|---:|
| Occupancy | 75% or higher |
| ADR | ₹5,000 or higher |
| RevPAR | ₹3,750 or higher |
| Cancellation Rate | 10% or lower |
| Guest Rating | 4.2 or higher |
| Check-in Delay | 15 minutes or lower |

> **Note:** These are training benchmarks for the assignment, not universal industry standards. Students should compare actual performance against the stated benchmark.

---

## 5. Required KPI Calculations

- **ADR**: `Room Revenue / Sold Room Nights`
- **RevPAR**: `ADR × Occupancy Rate`
- **Cancellation Rate**: `Cancelled Bookings / Total Bookings × 100`
- **Average Guest Rating**: `Average Guest Rating`
- **Average Check-in Delay**: `Average Checkin_Delay_Min`

---

## 6. Assignment Tasks

### Task 1 — Hotel Performance
Compare properties by bookings, revenue, occupancy and guest rating.
### Task 2 — Room Type Analysis
Compare Standard, Deluxe and Suite rooms using nights, revenue, ADR and occupancy.
### Task 3 — Booking Channel Analysis
Compare Direct, OTA, Corporate and Travel Agent bookings.
### Task 4 — Customer Segment
Compare Business, Leisure and Family customers by revenue, rating and cancellations.
### Task 5 — Monthly Trend
Analyze monthly occupancy, room revenue, bookings and cancellations.
### Task 6 — Revenue KPIs
Calculate ADR and RevPAR by hotel and room type.
### Task 7 — Service Quality
Compare complaints, guest ratings and check-in delays by hotel.
### Task 8 — Benchmark Analysis
Classify hotels against occupancy, ADR, RevPAR, cancellation and rating benchmarks.
### Task 9 — Hotel Dashboard
Build a management dashboard with hotel, room and channel slicers.
### Task 10 — Recommendations
Recommend actions to increase occupancy and revenue while improving guest experience.

---

## 7. Recommended Pivot Charts

1. **Revenue by Hotel** — Column Chart
2. **Occupancy by Room Type** — Bar Chart
3. **Revenue by Booking Channel** — Column Chart
4. **Monthly Occupancy Trend** — Line Chart
5. **Guest Rating by Hotel** — Bar Chart
6. **Cancellation Rate by Channel** — Bar Chart

---

## 8. Dashboard Requirements

Create a one-page professional dashboard containing:

### KPI Cards

- Bookings
- Room Revenue
- Occupancy %
- ADR
- RevPAR
- Cancellation Rate
- Guest Rating
- Average Check-in Delay

### Filters / Slicers

- Hotel
- City
- Room_Type
- Booking_Channel
- Customer_Type
- Month

### Dashboard Charts

- Revenue by Hotel
- Occupancy by Room Type
- Revenue by Channel
- Monthly Occupancy Trend

---

## 9. Final Business Questions

1. Which hotel generates the most revenue?
2. Which hotel has the highest occupancy?
3. Which room type performs best?
4. Which booking channel produces the most revenue?
5. Which channel has the highest cancellation rate?
6. Which hotel exceeds the RevPAR benchmark?
7. Which property has the best guest rating?
8. Where are service quality problems visible?
9. What three revenue-management actions should be taken?

---

## 10. Final Management Challenge

The hotel group wants to increase revenue without relying only on price increases. Identify the best-performing property, room category and booking channel and propose three operational changes.

---

## 11. Final Deliverable

Create an Excel workbook with:

1. **Raw Data**
2. **Analysis / Pivot Tables**
3. **KPI / Benchmark Analysis**
4. **Charts**
5. **Dashboard**
6. **Management Recommendations**

### Expected Workflow

```text
Raw Data
   ↓
Excel Table
   ↓
Pivot Tables
   ↓
Calculated KPIs
   ↓
Benchmark Comparison
   ↓
Pivot Charts
   ↓
Slicers / Timeline
   ↓
Dashboard
   ↓
Business Insights
   ↓
Management Decisions
```
