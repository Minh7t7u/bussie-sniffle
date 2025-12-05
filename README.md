# Sydney Bus Delay Prediction  
_A practical machine learning and data analysis project_



## Overview

Sydney bus services often run early or late compared to their scheduled times, creating uncertainty for commuters.  
This project explores whether those delays can be **predicted** using publicly available historical transport data.

The goal is to build a system that:

- Learns delay patterns from past bus behaviour  
- Predicts whether a future bus will be early / on-time / late  
- Eventually displays these predictions in a user-friendly way  
- Potentially integrates with tools commuters already use (e.g., Google Maps via a browser extension)

## Motivation

Unpredictable bus arrivals cost commuters time and reduce confidence in public transport.  
If we can identify consistent patterns such as:

- Peak-hour congestion  
- Route-specific delay trends  
- Day-of-week effects  
- Stop-level bottlenecks  

…then we can provide more realistic arrival expectations than the timetable alone.

A working predictor could help users:

- Avoid unnecessary waiting  
- Choose better departure times  
- Improve day-to-day planning  
- Make smarter commuting decisions  

This project tests whether such predictions are **feasible**, **useful**, and **accurate enough** to matter.

## Project Goals

### Short-Term (Current Phase)
- Download historical GTFS timetable + realtime arrival data  
- Clean and merge data to compute delays  
- Analyse patterns (peak hours, weekdays, routes)  
- Build a simple baseline predictor using historical averages  

### Medium-Term
- Train a lightweight machine learning model (tree-based regressor/classifier)  
- Compare ML performance to naive baselines  
- Build a small prediction API (e.g., using FastAPI)  

###  Long-Term Vision
- Combine real-time feeds + historical patterns for live predictions  
- Develop a browser extension overlaying predictions onto Google Maps  
- Provide commuters with clear, actionable insights:
  - “Expected arrival: 7:46pm (5–8 min late), confidence: 82%”

## Data Sources

Uses publicly available data from **Transport for NSW Open Data Portal**, including:

- **GTFS Static Timetables** – scheduled times  
- **GTFS-Realtime Trip Updates** – actual arrival/departure times  
- **Historical GTFS Archives** (where available)  

Data is used solely for research and educational purposes.


