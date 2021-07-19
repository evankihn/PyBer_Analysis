# PyBer_Analysis 

## Purpose 
Throughout our journey in this module we went through handfuls of options that involve using matplotlib and pandas to analyze, sort, and create meaningful visuals from complex datasets. The two csv files used for analysis were similiar in that they both contained a list of cities with the city_data showing the type of city (Urban, Suburban, and Rural) as well as the total amount of drivers in that city. By merging the two datasets, our purpose of the project was centered around better understanding the relationship between the city, the type, as well as the fare prices of rides in a four month span. 

## Development Enviornment
  - Jupyter Notebook 
  - Python (version 3.7)
      - Pandas library 
      - NumPy library
      - Matplotlib

## Analysis & Results
  - Analysis 
      - Before we got into developing any graphs or charts, we  began by summing important numbers that would help us see certain analytics between the types of cities involved. Using the codes below, we soon realized that the Urban population dominated the metrics when it came to totals, however, when it came to the average fare per ride and average fare per driver, the rates benefited drivers in the rural and suburban areas. 
          - "total_rides = pyber_data_df.groupby(["type"]).count()["ride_id"]"; "total_drivers = city_data_df.groupby(["type"]).sum()["driver_count"]";"fare_total = pyber_data_df.groupby(["type"]).sum()["fare"]"
          - "https://user-images.githubusercontent.com/82420244/126120829-04923e15-997b-40d4-9c5c-97d3a3725e5a.png"
    
      - From here, our path concerned more about the dates of the fares in relationship to the prices themselves between each type of city. As expected, the sum of all fares worked largest to smallest going from Urban -> Suburban -> Rural, respectively. 
          - https://user-images.githubusercontent.com/82420244/126121666-bcc7c570-66fa-4bb3-af0d-58d116347273.png
  
  - Results
      - Our second deliverable gave us brillant insight on where most of the fares saw an increase in dollar amount month to month. As stated in our analysis, we do realize that there is a huge discrepancy between the volume of all three city types, which obviously makes sense if you think about it. More rural areas are not going to see as much need for these drivers or rides, whereas urban populations are much more likely to use them in comparison. One interesting point to make out is that in the month of April, Suburban totals appear to be seeing a rigid uprise, while Urban totals see a steady decrease.
    
## Summary
For Pyber, it is clear there needs to be more of a continued shift to staying focused in Urban and Suburban areas. An alarming number, however, is the fact that the average fare paid to driver in rural areas is $55.49, while it is less than $20 in Urban areas. This absolutely could do with low volumes outside of the city, but it could also be observed that either fares need to be increased in Urban areas or drivers need to be moved out. Because the Urban market clearly is such a big part of Pyber's business, getting this fare per driver margin closer to its counterparts will balance the equation and more than likely increase sales for the company in the long term.
    