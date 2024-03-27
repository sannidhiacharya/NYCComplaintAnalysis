Project: NYC Complaint Analysis
This is a Python script for analyzing NYC complaint data retrieved from Socrata Open Data API.

Libraries:
- pandas
- sodapy
- numpy
- folium
- plotly.express
- collections
- requests

Data:
The script retrieves the first 1,000,000 rows of complaint data from NYC OpenData using Socrata API.

Analysis:
- The script focuses on complaints in the last 10,000 rows.
- It identifies Brooklyn as the borough with the most complaints.
- It performs the following analysis for Brooklyn:
    1.Breakdown of complaints by offense type (Radar plot)
    2. Statistical distribution of offenses (Violin plot)
- It creates three interactive Folium maps:
    Map 1: Complaint locations
    Map 2: Complaints by day of the week (color-coded)
    Map 3: Heatmap of complaint density

Instructions:
Replace client = Socrata("data.cityofnewyork.us", "...", "...", "...") with your own Socrata API credentials.
Update file paths in m.save("...") and map3.save("...") and map4.save("...") to your desired locations for saving the maps.
