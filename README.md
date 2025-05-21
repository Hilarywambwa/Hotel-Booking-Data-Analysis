# Hotel Booking Data Analysis

##Data is on Kaggle : https://www.kaggle.com/datasets/mathsian/hotel-bookings/data

## Project Overview
This Excel-based project analyzes booking data for two Portuguese hotels; a Resort Hotel in the Algarve and a City Hotel in Lisbon to drive strategic decision-making. The analysis focuses on optimizing revenue, reducing cancellations, enhancing marketing, and improving operational efficiency. Using data cleaning, pivot tables, visualizations, and an interactive dashboard, the project delivers actionable insights tailored to each hotel's needs.

## Business Problem
The hotels aim to:
- **Maximize Revenue**: Optimize pricing based on lead times and stay patterns.
- **Enhance Marketing**: Target low-cancellation segments and boost loyalty.
- **Reduce Cancellations**: Address high cancellation rates in specific segments.
- **Improve Operations**: Streamline booking processes and tailor amenities.

## Dataset
The dataset includes booking details such as:
- **Columns**: `hotel`, `market_segment`, `lead_time`, `stay_in_weekend_nights`, `stay_in_week_nights`, `no_of_adults`, `no_of_children`, `no_of_babies`, `is_repeated_guests`, `previous_cancellations`, `booking_changes`, `days_in_waiting_list`, `total_of_special_requests`, `is_canceled`.
- **Source**: Hotel booking records for Resort and City Hotels.

## Data Preparation
- **Cleaning**:
  - Removed duplicates based on all columns.
  - Excluded 2 rows with "Undefined" in `market_segment`.
  - Replaced blank `no_of_children` with 0.
  - Converted `is_canceled` (0, 1) to "Retained," "Canceled."
  - Converted `is_repeated_guests` (0, 1) to "One time guest," "Repeated guest."
- **Validation**: Ensured numeric columns (e.g., `lead_time`) and binary columns were correctly formatted.

## Analysis
- **Pivot Tables**:
  - Cancellation rates by `market_segment` and `hotel`.
  - Average `lead_time` by `hotel` and `market_segment`.
  - Stay patterns (`stay_in_weekend_nights`, `stay_in_week_nights`) by `hotel` and `no_of_adults`.
  - Proportion of `is_repeated_guests` by `market_segment` and `hotel`.
- **Visualizations**:
  - Clustered bar chart: Booking status (Retained/Canceled) by `market_segment`.
  - Line chart: Average `lead_time` by `market_segment`.
  - 100% stacked column chart: Week vs. weekend nights by `market_segment`.
  - Clustered column chart: One-time vs. repeat guests by `market_segment`.
  - Pie charts: Sum of `total_of_special_requests` and `booking_changes` by `market_segment`.
- **Dashboard**: Interactive with slicers for `hotel` and `market_segment`, displaying key metrics (total bookings, cancellation rate, lead time, stay duration, repeat guest proportion).

## Key Insights
- **Revenue Management**:
  - Resort Hotel: Longer lead times (e.g., 155 days for Groups) support early-bird pricing.
  - City Hotel: Shorter lead times (e.g., 99 days for Offline TA/TO) suggest last-minute promotions.
  - Weekday bookings dominate, indicating business-driven demand.
- **Marketing Strategy**:
  - High cancellation rates: Groups (44% City, 40% Resort), Online TA (41% City, 40% Resort).
  - Low cancellation rates (<20%): Direct, Corporate, Complimentary segments.
  - Groups, Online TA, and Offline TA/TO show higher repeat guest rates, justifying loyalty programs.
- **Cancellation Reduction**:
  - Groups and Online TA have high cancellation rates; require non-refundable deposits.
- **Operational Efficiency**:
  - Frequent `booking_changes` in Online TA suggest clearer booking policies.

## Recommendations
1. **Revenue Management**:
   - Resort Hotel: Implement early-bird pricing for bookings 90+ days out.
   - City Hotel: Offer last-minute discounts for bookings within 30 days.
   - Both: Enhance weekday business packages (e.g., meeting rooms, breakfast).
2. **Marketing Strategy**:
   - Shift focus to Direct and Corporate segments with low cancellation rates.
   - Develop loyalty programs for Groups and Online TA with rewards (e.g., discounts, priority booking).
3. **Cancellation Reduction**:
   - Introduce non-refundable deposits for Groups and Online TA.
   - Streamline booking systems with clear cancellation terms.
4. **Operational Efficiency**:
   - Clarify booking policies to reduce `booking_changes` in Online TA.
   - Offer business traveler amenities (e.g., Wi-Fi, express check-in).


## Conclusion
This project empowers the Resort and City Hotels to make data-driven decisions, optimizing revenue, reducing cancellations, and enhancing guest satisfaction. The interactive dashboard and detailed analysis provide stakeholders with clear, actionable strategies to drive profitability.

![image](https://github.com/user-attachments/assets/ad3c54cf-3544-4fdb-af31-397254399ef1)

