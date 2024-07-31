DATASET: https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data

Data Initial Observations:

  Empty or error values in all columns except name column.
  49080 rows and 16 columns in data.
    
Preprocessing and data cleaning:

  1. column id is removed for facilitating better data cleaning- total columns changed to 15.
  2. error rows and blank rows are removed- total rows changed to 48894.
  3. 168 empty rows in host_id have data only on name column with 15 null column so they are removed- total rows changed to 48726.
  4. empty rows in name column is removed- total rows changed to 48710.
  5. 21 blank rows n host_name is replaced with value "unspecified".
  6. 10026 null values in last_review and reviews_per_month:
       last_review null values replaced with mode value=6/24/2019
       reviews_per_month null values replaced with approximate column average=0.93
  7. An index column starting from 1 is added to the data and column for reference purposes.
  8. Number of rows after cleaning-48710, Number of columns after cleaning-16.

  Managing Relationships: 
  
  Since there is only one column, there is no need for establishing relationships.

Visualsations:

  1. Map with latitude and longitude of airbnb listings as reference.
  2. Stacked column chart(Neighbourhoods vs Count of listings).
  3. Pie chart(Neighbourhood groups/No of airbnb listings).
  4. Stacked column chart(Room type vs No of reviews).
  5. Stacked column chart(Neighbourhood groups vs No of reviews).
  6. Pie chart(Month of last review/No of airbnb listings).
  7. Stacked column chart(Neighbourhood groups vs Average of availability per 365).
  8. Stacked column chart(Neighbourhood groups vs Average price).
  9. Line and stacked column chart(Neighbourhoods vs Price,Average of availability per 365).

Insights:
  1.Manhattan has the highest number of airbnb listings(44.34%) closely followed by Brooklyn(41.02%) in neighbourhood groups and Staten Islands has the least listings.
  2.Williamsburg in Brooklyn has the highest number of listings(3912) in neighbourhoods. Of the top 20 neighbourhoods, 7 belong to Brooklyn,12 belong to Manhattan, 1 belong to Queens.
  3.From the room types, most reviews are about entire home/apartment(577911) and private rooms(535947).
  4.Brooklyn has the most reviews(485575) followed by Manhattan(452502).
  5.Last reviews were seem to be mostly in the month of June(53.58%) with July(13.29%) being the next most recurring month.
  6.The average of minimum nights required for booking is highest in Manhattan(8.54) and lowest in Bronx(4.59).
  7.From neighbourhood groups, Staten Island has the highest average availability per year(198.36) and Brooklyn being lowest(100.15).
  8.Manhattan has the highest average price per listing(196.73) and Bronx(87.69) the lowest. Brooklyn has significantly lower average price(124.41) when compared with Manhattan.
  9.Williamsburg in Brooklyn has the highest total price of airbnb listings(562790).Of the top 20 neighbourhoods, 6 from Brooklyn,13 from Manhattan,1 from Queens.
  10.Woodrow, Bay terrace, New Dorp has no availability in 365 days. Fort Wordsworth has whole year availability.
