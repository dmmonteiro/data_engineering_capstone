## Data Dictionary

This document describes the data dictionary for the proposed star schema.

### Arrivals
column name | description
---: | :---
| id | arrival unique id |
| port | port of entry code |
| arrival_date | immigrant arrival date |
| departure_date | immigrant departure date |
| mode | arrival mode (e.g. land, air, etc.) |
| visa | visa code |
| visatype | visa type |
| age | age of the immigrant |
| gender | gender of the immigrant |
| airline | airline code |
| flight_num | flight number |
| occupation | occupation of the immigrant |
| admission_num | admission number |
| country | code of visitor's country of origin |

### Visa
column name | description
---: | :---
| type | visa type (WT, B1, ...) |
| purpose | visa purpose (Business, Pleasure, etc.)|
| code | visa i94 code |
| description | visa description |

### arrival_mode 
column name | description
---: | :---
| code | arrival mode code |
| description | mode description (e.g. Air, Land, etc.)|

### Calendar
column name | description
---: | :---
| date | date in the format YYYY-MM-DD |
| day | day in numeric value |
| week_day | week day in string format|
| month | month in numeric value |
| month_name | month name in string format |
| quarter | year quarter |
| year | year as numeric value |
| season | season as numeric value |
| season_name | season name in string format|

### Ports
column name | description
---: | :---
| code | port of entry code |
| city | port of entry city |
| state | port of entry state |

### Airlines
column name | description
---: | :---
| name | airline company name |
| code | IATA code |
| country | country of origin|

### Countries
column name | description
---: | :---
| code | country code |
| country | country name |

### Temperatures
column name | description
---: | :---
| city | US city|
| month | month as a 1-12 number |
| avg_temp | historical average temperature per month |