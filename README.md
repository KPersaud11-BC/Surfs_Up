# Surfs_Up Analysis by Kieran Persaud

## Overview of the Surf's Up Challenge
In the Challenge scenario, I am looking to open a Surf and Shake Shop that would serve ice cream year-round in Hawaii. After meeting with W. Avy, an investor who wants to back my venture, he shares concerns about the effects of the weather on the viability of the business. In the Challenge, he asks me to run weather analytics on data from Oahu for June and December, in order to determine if the surf and ice cream shop business is sustainable year-round.

## Resources
**Data Sources:** ```hawaii.sqlite```

**Software:** Anaconda 4.10.1, Pandas, json, numpy, time and sqlalchemy Libraries, PythonData kernel; Jupyter Notebook

## Results
The following table was created from the Measurements table in the ```hawaii.sqlite``` file, filtered by June and December.
<table>
  <tr>
    <td>June Temps</td>
   <td>December Temps</td>
  </tr>
  <tr>
    <td><img src="https://user-images.githubusercontent.com/84286467/129489503-85902baa-da2f-4717-8d0b-dac2cb3c7e72.PNG" width=140 height=265></td>
    <td><img src="https://user-images.githubusercontent.com/84286467/129489534-bb63520e-e244-4ec5-9c70-b85594b54f77.PNG" width=160 height=275></td>
  </tr>
 </table>

There are several key differences in weather data between June and December are the following:
- June has approximately 200 more data points than December.
- The average temperature in June (74.9) is approximately 4 degrees higher than the average temperature in December (71.0).
- The standard deviation of December Temperatures is higher than that of June. This implies that there is greater variance and range in December temperature data.
- Both June and December data have a similar max temperature.

### Additional Queries
One additional query that can be done is gather more data for December. As mentioned, June has 200 more data points than December. The current data ends in August 2017, so it excludes December 2017. This may level out any average or standard deviation discrepancies that showed up in my key differences.

Another additional query that can be done is analyzing precipitation. I wrote a query in a similar manner to the challenge deliverables that described precipitation data for June and December. The resulting table is show below.
<table>
  <tr>
    <td>June Precip</td>
   <td>December Precip</td>
  </tr>
  <tr>
    <td><img src="https://user-images.githubusercontent.com/84286467/129489503-85902baa-da2f-4717-8d0b-dac2cb3c7e72.PNG" width=140 height=265></td>
    <td><img src="https://user-images.githubusercontent.com/84286467/129489534-bb63520e-e244-4ec5-9c70-b85594b54f77.PNG" width=160 height=275></td>
  </tr>
 </table>
