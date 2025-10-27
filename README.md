# Mobile-Device-Usage-and-User-Behavior

## This Power BI dashboard provides a detailed analysis of user behavior across different mobile operating systems, demographics, and usage patterns.
<hr>

## Dashboard Objective

### -To compare usage and resource consumption (data usage and battery drain) between Android and iOS user bases.

### To identify user segments (by Age and Gender) driving the highest Screen Time and Data Usage.

### To correlate the number of installed applications with daily data consumption.
<hr>

## Key Data Points & Metrics

### Sum of Data Usage (MB/day): Total data consumed, broken down by Operating System (OS).

### Sum of Screen On Time (hours/day): Total accumulated screen time, segmented by Age group.

### Battery Drain in Different Devices (K): A comparison of resource consumption across top device models (e.g., iPhone 12, Xiaomi Mi 11).

### User Behavior Class: A slicer for segmenting users by pre-defined behavioral cohorts.
<hr>

<img src="dashboard ss\dashboard1.PNG" alt="Full Dashboard">
<hr>
<img src="dashboard ss\dashboard2.PNG" alt="Data of Ios device">
<hr>
<img src="dashboard ss\dashboard3.PNG" alt="Data of Level 3 Android device usage">
<hr>

## Core Insights & Findings

### OS Dominance: Android users account for the majority of the data usage (78.34% of the total volume).

### Power Users: Users with a high number of installed apps (specifically 80–100 apps) are the most significant data consumers across both platforms.

### Peak Screen Time: The highest total screen time is seen in the 20s and 30s age groups, with another high point in the 50s age group.

### Android Profile: The analyzed sample showed a demographic skew toward Male (75%) Android users, with the highest screen time observed in the 50–55 age range.

### iOS Profile: iOS users in the sample show a more balanced Gender split and peak screen time in the 55–60 age group.
<hr>

## some Insights

## 1. Validate and Standardize Screen Time Metric

### Current Issue: The chart "Sum of Screen On Time (hours/day) by Age" displays a Sum of hours (e.g., 162 hours for age 30)1, which is misleading as it represents the total time across an entire group, not the typical individual usage. This makes comparisons between groups of different sizes unreliable.

### Next Step Description:The underlying DAX (Data Analysis Expressions) measure for the "Screen On Time" visual must be changed from a $\text{SUM}$ calculation to an $\text{AVERAGE}$ calculation. This will ensure the visual displays the Average Screen Time per User (hours/day) for each age bracket. This change will provide a true representation of engagement and allow for fair, comparative analysis of how different demographics utilize their mobile devices.