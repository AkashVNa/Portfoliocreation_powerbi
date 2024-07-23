DATASET: https://www.kaggle.com/datasets/dgomonov/new-york-city-airbnb-open-data

Data Initial Observations:

  Empty or error values in all columns except name column.
  49080 rows and 16 columns in data.
    
Preprocessing and data cleaning:

  column id is removed for facilitating better data cleaning- total columns changed to 15.
  error rows and blank rows are removed- total rows changed to 48894.
  168 empty rows in host_id have data only on name column with 15 null column so they are removed- total rows changed to 48726.
  21 blank rows n host_name is replaced with value "unspecified".
  10026 null values in last_review and reviews_per_month:
      last_review null values replaced with mode value=6/24/2019
      reviews_per_month null values replaced with approximate column average=0.93
  An index column starting from 1 is added to the data and column for reference purposes.
  Number of rows after cleaning-48726, Number of columns after cleaning-16.

  
