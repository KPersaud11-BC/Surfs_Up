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

## Summary
### Additional Queries
One additional query that can be done is gather more data for December. As mentioned, June has 200 more data points than December. The current data ends in August 2017, so it excludes December 2017. This may level out any average or standard deviation discrepancies that showed up in my key differences.

Another additional query that can be done is analyzing precipitation. I wrote a query in a similar manner to the challenge deliverables that described precipitation data for June and December. The resulting table is shown below.
<table>
  <tr>
    <td>June Precip</td>
   <td>December Precip</td>
  </tr>
  <tr>
    <td><img src="https://user-images.githubusercontent.com/84286467/129493446-a54f8cf7-eb55-47b3-846b-917e7cf9ed61.PNG" width=200 height=300></td>
    <td><img src="https://user-images.githubusercontent.com/84286467/129493452-dd2c6b5e-0e3c-4118-a46a-c04463fd3a8b.PNG" width=200 height=300></td>
  </tr>
 </table>
I also read the Measurement data from SQL to a DataFrame and exported it to Excel. There I ran an additional query regarding the amount of days in each month that experienced precipitation. The resulting table is shown below.

![Table](https://user-images.githubusercontent.com/84286467/129493606-5585ed23-a22b-4e46-8258-182bd3a7546b.PNG)

From these two results, one can determine that December experiences a higher average precipitation than June, and that it experiences more days of precipitation as a percentage of its total data.
