# Geolocation Database (MSSQL, T-SQL)

This repository contains an SQL query that creates the necessary tables for location services, and inserts all real-life information of:

- Regions
- Subregions
- Countries
- States
- Cities

All tables include Latitude and Longitude values for computing the columns' map pointing at its location on your project. 

### Each **subregion** has a FK for *regions*, **country** has FK's for *regions* and *subregions*, **state** for *countries*, and **cities** for *states* and *countries*. 

## Shared columns (Will not be included in the upcoming table descriptions !!!):
- Id,
- Name,
- Translations,
- Latitude,
- Longitude,
- Created at,
- Updated at,
- Geo Flag

#### **(Also the contents of regions table)**

## Subregions table includes:
- Region ID

## Countries table includes: 
- Region ID, Subregion ID,
- Country codes by Alpha 2, Alpha 3 codes (ISO 3166),
- Phone code,
- Numeric codes,
- Capital,
- Currency name and symbol,
- Native, Nationality
- Top-level domain,
- Timezones

## States table includes:
- Country ID,
- State code by Alpha 2 (ISO 3166-2),
- FIPS code

## Cities table includes:
- State ID, State code,
- Country ID, Country code
  
