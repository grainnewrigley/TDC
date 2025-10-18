---
title: 'Understanding Environmental Data: A Beginners Guide'
date: 2025-10-18
permalink: /posts/2025/02/environmental-data-beginners-guide/
tags:
  - data analysis
  - resource
---

This beginners guide will teach you about the different types of environmental data and how to interact with them.

The simplest definition of environmental data is information about the environment. It can mean a huge number of things - a photo of a park, a temperature reading, a chemical detection. Most often when we talk about environmental data, we mean a series of organsied data, such as measurements over a period of time, often collected as part of research. Environmental data is crucial for deepening our understanding of our ecosystem and tracking our footprint to ensure a sustainable planet for future generations. 

If you’re like me, fascinated by the environment and wanting to put your analytical skills to good use, you might be interested in looking at environmental data. This guide is a good place to get started with definitions, resources, and project ideas. I gathered this information from my Data Analysis Level 4 Apprenticeship and the internet. When you’re ready to handle some data, have a look at our open source environmental data library. 

<h2>Data Vocabulary</h2>

**Qualitative Data** - Non-numeric data, e.g., videos, text. <br>
**Quantitative Data** - Numeric data, e.g., numbers, decimals.

**Continuous Data** - Data that sits on a spectrum, e.g., temperature, height. <br>
**Discreet Data** - Data in separate categories, e.g., days of the week, colours.

**Spreadsheet** - an electronic document where data is arranged in the rows and columns of a grid, and can be manipulated and used in calculations.


<h2>Types of Environmental Data</h2>
Environmental data can represented in several ways:

**1. Tabular Data**

This is data organised in rows and columns, similar to a spreadsheet. It may include spatial (distance/area) or temporal (time) information. This is the most common way data is stored, and is the easiest kind of data to work with for beginners. Look for files like .csv or .xslx.
Examples: Chemical analysis of water samples, species observation lists, results from environmental surveys.

**2. Spatial Data**

This data relates to a specific location on Earth. This is separate from tabular data because it’s not stored in a table, but in something that represents the area, like a photograph or map. It's often divided into two sub-types:

**Raster Data:**
Data stored in a grid of pixels (like an image). Each pixel has a value representing an area.
Examples: Satellite imagery, digital elevation models (DEMs), gridded climate data (temperature maps).

**Vector Data:**
Data stored as geometric shapes: points (0 dimensional), lines (1 dimensional), and polygons (2 dimensional).
Examples: Locations of monitoring stations (points), rivers or roads (lines), park boundaries or state borders (polygons).

**3. Time-Series Data**

This is data collected sequentially over time, often at regular intervals. It's crucial for tracking trends and changes. This can be a type of tabular data where each row is something being tracked and each column is a reading at a certain time.
Examples: Hourly air quality readings, daily precipitation totals, monthly average temperatures, annual population surveys of a species.

<h2>Common File Types for Environmental Data</h2>
These are some of the most common file types for environmental data. Spreadsheets - used for tabular data, time-series data, and more - are the most common and easiest for beginners to work with. There are also some specialised file formats that can store large, complex datasets, especially those with spatial and time-series components.

**1. Spreadsheets and Text**

**Comma Separated Values (.csv):** The most common simple text-based format for tabular data. Easy to read and widely supported. Best for simple monitoring data. Use excel, google sheets, Python (pandas), or R (Tidyverse)

**Microsoft Excel (.xlsx):** Excellent for smaller datasets and initial data cleaning, but less scalable for huge or complex spatial data.

**ASCII Text (.txt):** Plain text files, sometimes used for simple gridded or numerical data.

**2. Geospatial and Climate Formats**

These are some of the most common specialised file formats, along with the tools best suitable for working with them. These formats are "self-describing," meaning the file includes not just the data, but also metadata (data about the data) like the coordinates, units, and collection methods.

| File Type                          | Purpose                                                                                                                                                                                         | Key Benefit                                                                                          | Tool                                                       |
|------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|------------------------------------------------------------------------------------------------------|------------------------------------------------------------|
| GeoTIFF (.tif)                     | A popular format for raster data (satellite images, gridded models). The "Geo" means it contains georeferencing information.                                                                    | Widely compatible with GIS software; stores spatial location.                                        | Python (Rasterio/GDAL) or R                                |
| Shapefile (.shp, .shx, .dbf, etc.) | A standard format for storing vector data (points, lines, polygons) used in Geographic Information Systems (GIS). Note: A Shapefile is actually a collection of at least three essential files. | Essential for mapping and spatial analysis; stores geometry and attributes (data).                   | QGIS (beginner friendly), ArcGIS Pro or Python (Geopandas) |
| NetCDF (.nc, .nc4)                 | Network Common Data Form. Designed to store large, multidimensional array-oriented data, commonly used for climate models and weather data.                                                     | Highly efficient for storing time-series and gridded data (like x, y, z, and time); self-describing. | Python (Xarray/NetCDF4) or R                               |
| HDF (.hdf, .hdf5)                  | Hierarchical Data Format. Similar to NetCDF but often more complex. Used extensively by NASA and other organisations for Earth observation data.                                                | Can store massive and diverse data types within one file.                                            | Python (h5py/NetCDF4) or R                                 |


<h2>Tools for Environmental Data Analysis</h2>
These are some of the most common tools for environmental data analysis

**1. Spreadsheet & Tabular Analysis**

**Microsoft Excel:** Excellent for cleaning, sorting, basic calculations, and simple visualisations of tabular data. This is the industry standard for working with tabular data, and ‘the second best tool for any job’ (as it can do any job almost as well as a specialised tool).

**Google Sheets:** Free version of Microsoft Excel.

**2. Programming Languages**

If you want to perform complex analysis, statistical modeling, and automate tasks, programming is key. 

**Python:**
The industry standard for data analysis. It is easy for beginners to learn as it mainly uses plain english. It has useful libraries for environmental data:

- **Pandas:** For data manipulation and cleaning.
- **NumPy:** For numerical operations (using ‘arrays’).
- **Matplotlib/Seaborn:** For data visualisation.

**R:**
Also popular for data analysis, more useful for statistical analysis and generating high-quality statistical graphics.

**SQL:**
Honorable mention, Structured Query Language is common in data analysis and specifically used for parsing data in SQL databases. This is a common data analysis tool. 

**3. Geographic Information Systems (GIS) Software**

These tools are specifically designed to analyse, manage, and visualise spatial data.

**QGIS:**
A free and open-source GIS tool for spatial data analysis. GIS is a technology that links data to a map, allowing users to create, manage, analyse, and visualise geographic information. It is powerful, widely used, and has excellent community support, perfect for beginners.

**ArcGIS Pro:**
The industry standard, a paid GIS tool for spatial analysis

**4. Interactive and Visualisation Tools**

**Jupyter Notebooks:**
An interactive environment (often used with Python/R) that lets you write code, create visualisations, and add explanatory text in a single document. Perfect for website content.

**Tableau/Power BI:**
Dedicated Business Intelligence (BI) tools for creating interactive dashboards and visualisations that can be embedded or shared on your website.

<h2>Your First Data Analysis Project</h2>
To turn data into compelling website content, the Data Analysis Lifecycle provides a helpful project structure:

**1. Define Your Story and Audience**

Before starting with the data, consider what environmental story you want to tell. What question are you looking to find an answer to? For example: How has air quality changed in my city over the last five years?

Also consider your audience and their technical level. Who is this information meant to serve, and what is the best way to communicate it to them? For example: The general public living in my city (avoid jargon, use visualisations, focus on impact)

**2. Acquire and Clean the Data**

**Acquisition:**
Find data from reputable sources. Look online for open source data from government agencies, research institutions, official open-source portals like NASA Earthdata, your local environmental protection agency, or the Two Degrees Cooler Environmental Data Library. 
Finding data is a key skill for data analysts. A big part of the job is finding the right data, ensuring it has the necessary license, and gaining access to it. 

**Cleaning:**
This is often the most time-consuming step. It is estimated to take 80% of a project’s time. Use tools like Excel or Pandas (Python) to:
Handle missing values (gaps in the data).
Standardise units (e.g., converting Celsius to Fahrenheit).
Filter out irrelevant, erroneous, or anomalous readings.

**3. Analyse and Visualise**

**Analysis:**
Calculate trends, averages, totals, and correlations using your chosen tool  - R, python, SQL, Power BI, etc. There’s a lot you can do with this. If you’re stuck for ideas, start with statistical analysis like mean, sum, minimum, etc. 

**Visualisation:**
Create charts, graphs, and maps that clearly illustrate your findings.
For time-series: Line charts show trends over time.
For spatial data: Maps created in QGIS or Python/R show where things are happening.
For comparative data: Bar charts or pie charts.

**4. Present and Publish**

**Contextualise:** Every data project should come with an explanation. Think about your target audience and their technical expertise when you write this. You can use the Jupyter Notebook format to write narrative text alongside your code and results, or write an explanation alongside an image. 

**Interactive Maps/Charts:** With some practice, you can use Python libraries (like Leaflet or Plotly) or BI tools (like Tableau Public) to create interactive visualisations. Interactive elements (like hover-over details) are great for engagement. 

**Embed:** Most visualisation tools provide an embed code (like a YouTube video) that you can paste directly into your website's HTML to display the interactive results.


In this beginner's guide, we have covered:
- Data vocabulary
- Environmental data types
- Environmental data files
- Environmental data tools
- The data analysis lifecycle. 

I hope this is a useful resource for anyone getting started with environmental data analysis, especially self-taught data analysts or those using open source data. Please get in touch if you have found this helpful, or have anything to add! 


