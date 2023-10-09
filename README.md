# Optimizing the Timing of Insulin Injections
Data processing and analysis for ["Determining the optimal timing for insulin injection to minimize glucose level variability after a meal in ideal conditions"](https://users.aalto.fi/~keimiom1/portfolio/writing/determining-the-optimal-timing-for-insulin-injection-to-minimize-glucose-level-variability-after-a-meal-in-ideal-conditions.html) - a research project for the IB Standard Level Mathematics Analysis and Approaches course inspired by my type 1 diabetes. 

With type 1 diabetes, there are broadly two major problems that must be solved daily by the diabetic individual: when to eat or inject insulin and how much?
This research aimed to answer the former question using my personal CGM data collected between 27.10.2021 and 1.12.2021.

The overall method was to isolate the events where I naturally either injected 1 unit of insulin or consumed 10 grams of carbohydrates far enough from eating
and exercise from the over 10 000 data points that my dexcom G6 glucose sensor collected over the data collection period. I used statistical methods to model
the average behavior of my glucose levels in those events to produce curves (functions) for both types of events with python. Adding together the curves and
taking the integral of that graph with different x-offsets of the insulin injection curve then produced the optimal timing with the simplified assumptions
that were made. Due to these simplified assumptions and the one person test group, the results are not to be trusted in making medical decisions but the
process may be used as inspiration for a better algorithm one day.

Read more about the results and process here: [https://users.aalto.fi/~keimiom1/portfolio/writing/determining-the-optimal-timing-for-insulin-injection-to-minimize-glucose-level-variability-after-a-meal-in-ideal-conditions.html](https://users.aalto.fi/~keimiom1/portfolio/writing/determining-the-optimal-timing-for-insulin-injection-to-minimize-glucose-level-variability-after-a-meal-in-ideal-conditions.html)
