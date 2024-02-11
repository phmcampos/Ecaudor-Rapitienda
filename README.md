# Ecuador JOKR Sales Exploration

## Overview

This repository contains an analysis of the JOKR sales dataset in Ecuador. The analysis aims to understand sales patterns and factors influencing sales for the grocery and delivery platform. 

## Motivation

The analysis is driven by the need to optimize sales strategies and enhance the delivery experience for JOKR customers in Ecuador. By exploring the dataset and addressing specific business questions, actionable insights can be derived to maximize sales effectiveness and improve customer satisfaction.

## Libraries Used

- pandas
- numpy
- seaborn
- matplotlib
- datetime
- missingno
- statsmodels
- scipy

## Files in the Repository

- **train.csv**: Sales dataset containing information about total product sales by store, product family, and date, including details on promotions.
- **stores.csv**: Dataset providing store information, including geographic data and store categorizations.
- **holidays_events.csv**: Dataset containing information about special dates that may influence family expenses throughout the year.
- **oil.csv**: Dataset including oil price data, relevant due to Ecuador's oil-dependent economy.

## Analysis Summary

### Business Understanding

JOKR is a grocery and delivery platform operating in the USA and Latin America, with a focus on hyper-local product delivery services. The analysis addresses three key business questions:
1. Effectiveness of promotion strategies in maximizing sales.
2. Sales seasonal patterns in Ecuador.
3. Key factors influencing JOKR's total sales in Ecuador.

### Exploratory Data Analysis and Data Modeling

To address the business questions, the analysis followed the Cross Industry Standard Process for Data Mining (CRISP-DM) methodology, encompassing exploratory data analysis (EDA) and data modeling techniques.

1. **Promotion Strategy Effectiveness**: Linear regression analysis revealed that promotion significantly improves sales, with a log transformation of the promotion variable yielding better model performance.
2. **Sales Seasonal Patterns**: Seasonal patterns were identified through STL decomposition and statistical tests, revealing significant variations in sales based on month, month day, and weekday. December and payday periods emerged as particularly important factors influencing sales.
3. **Key Factors Influencing Sales**: Linear regression analysis identified days of the week, December, payday periods, and supply issues as the most important factors influencing JOKR's total sales in Ecuador. Promotion and oil price also showed significant but less pronounced effects.
