# Temeperature API 

This API is created using Python, Pandas, and Flask to provide temperature data for different states during various eras based on years. The API allows users to retrieve temperature values for each state along with the relevant dates.

## Requirements
To run this API, make sure you have the following requirements installed:

- Python 3.x
- Pandas
- Flask

## Data Format
The temperature data is stored in a CSV file and loaded into a Pandas DataFrame. Each row represents a temperature record and includes the following columns:

- Station: The ID of the weather station.
- Date: The date of the temperature record.
- Temperature: The temperature value for the corresponding station and date.

## Example

#### Retrieve the temperature for a specific station on a specific date:
```
GET http://localhost:5000/api/v1/10/1988-10-25
```

- This will return the temperature value for station 10 on October 25, 1988.

#### Retrieve the temperature values for a specific station for all dates:
```
GET http://localhost:5000/api/v1/10
```
- This will return the temperature values for station 10 for all available dates.

#### Retrieve the temperature values for a specific station for a given year:
```
GET http://localhost:5000/api/v1/yearly/10/1998
```
- This will return the temperature values for station 10 for the year 1998.