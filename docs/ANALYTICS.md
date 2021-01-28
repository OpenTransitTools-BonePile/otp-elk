### What Analytics to Capture from server logs and trip requests.

1. Origin/Destination (O/D) studies:
   - what common places do people travel from or to (so individual O and D)
     - top N places people travel from or to on TriMet
     - top N places people who change modes travel to
     - top N places people travel from/to at night
     - on a Friday or Saturday night 
   - is there a time element:
      - commuter inflow and outflow to the city
      - people travel to the airport when ?  the hospital when?
   - are there O/D pairs that show up often?

1. MODE study:
   - what modes and combo of modes do people use
      - raw mode counts
      - repeat user .. do they change modes?
   - MODE and time of day /  day of week
     - do people travel on Uber in the night time
     - do people mostly travel on BIKETOWN / e-scooter or bike during the day
   - MODES and locations
     - do certain modes cluster in certain locations

1. trip planner patterns (Marshall):
    - ?

1. combo with and/or other data:
    - hop taps (Marshall)
       - hop taps to stops?
       - O/D study from HOP
       - HOP data is already matched to stops (at least the 'on's).  
       - Mike G's unaware of any OD studies being used with this data tho.
    - 

1. Raw Counts: 
   - which end user apps (main site, call center, 3rd party apps)
   - monitoring and validation (Marshall)
   - mobile or desktop
   - how successful was the request 
      - get a response back?
      - get a response with desired modes?
      - 
   
### What Systems would best capture this stuff?
 - ELK
   - what views does Kabana have for O/D, etc...?
   - how to load URL params into ES?
 - ELK + custom data loaders and views ?
 - PostGIS + D3js
   - https://blog.bitsrc.io/11-javascript-charts-and-data-visualization-libraries-for-2018-f01a283a5727
   - https://medium.com/@Elijah_Meeks/d3-is-not-a-data-visualization-library-67ba549e8520
 


### Other:
  - IMI Data Plan:
    - https://drive.google.com/drive/u/0/folders/1gLi7IJELh1f_Z4FRvivAEBiIAFoR1enu
    -
  - Provide some high level updates
      - OTP metrics data
      - brief data dictionary
      - file location
      - API enabled or other export function. 
  - Curious are you enabling a reverse geocoding to scrub out addresses and set the number of decimals for lat/long to appropriately anonymize location?
