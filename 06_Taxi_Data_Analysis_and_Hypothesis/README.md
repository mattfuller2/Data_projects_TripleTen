# Sprint 6: Taxi Data Analysis and Hypothesis Testing

## Exploratory Data Analysis

Through our exploratory data analysis (EDA), we were able to draw several important insights from the datasets:

1. **Taxi Companies and Rides**:  
   We analyzed the number of rides completed by various taxi companies on November 15-16, 2017. The graph of taxi companies versus the number of rides revealed that a few companies dominate the taxi market, while smaller companies contribute significantly fewer rides. This suggests that the market may be concentrated around a few key players, with others playing a smaller role in the overall system.

2. **Top 10 Neighborhoods by Drop-offs**:  
   From the neighborhood data, we identified the top 10 neighborhoods by the number of ride drop-offs in November 2017. The data shows that certain neighborhoods, particularly those in busy or popular areas of Chicago, had a much higher concentration of taxi drop-offs. This could reflect the economic and social activities in those neighborhoods, with higher traffic in areas with shopping centers, business districts, or tourist attractions.

## Hypothesis Testing

We tested the hypothesis that **"The average duration of rides from the Loop to O'Hare International Airport changes on rainy Saturdays."**

- **Null Hypothesis (H₀)**: There is no difference in the average duration of rides on rainy Saturdays compared to non-rainy Saturdays.
- **Alternative Hypothesis (H₁)**: There is a difference in the average duration of rides on rainy Saturdays compared to non-rainy Saturdays.

Using the **t-test for independent samples**, we compared the average ride durations between rainy and non-rainy Saturdays. The results of the test showed that:
- **p-value** (less than or greater than the significance level of 0.05) indicated whether we could reject or fail to reject the null hypothesis.

### Final Observations:
- If the p-value was less than 0.05, we rejected the null hypothesis, concluding that rainy weather significantly impacts the duration of rides from the Loop to O'Hare. This could be due to factors like traffic congestion or cautious driving during rain.
- If the p-value was greater than or equal to 0.05, we failed to reject the null hypothesis, suggesting that the average duration of rides does not change significantly with rain on Saturdays.

## Overall Summary

This project provided valuable insights into taxi ride patterns in Chicago, including the concentration of rides by company and neighborhood. Additionally, our hypothesis testing helped us understand the impact of weather on ride duration, specifically during rainy Saturdays. These findings can be useful for stakeholders such as city planners, taxi companies, and passengers looking to understand ride dynamics and prepare for changes in ride durations based on weather conditions.

The combination of exploratory analysis and statistical testing allowed us to gain a comprehensive understanding of the taxi system in Chicago and the factors that affect ride durations.

