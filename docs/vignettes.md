# Vignettes

## Sea ice

Arctic sea ice influences global atmospheric patterns and oceanic thermohaline circulation and, due to its high albedo, regulates the planetary energy balance. ICESpark enables users to mine multiple large datasets for use in remote sensing algorithm development and verification (validation tasks).

#### Example 1

ICESpark users can write a Spatial SQL query in Jupyter Notebook to extract coincidental ICESat-2 orbits around a SODA point.

<img src="/images/sea-ice.png" width="250" style="float:right;clear: right">

```sql
SELECT O.orbit, O.name, O.timerange
FROM Orbit_tbl AS O, SODA_tbl AS SODA
WHERE Spatial_Overlaps (O.orbit, SODA.location)
```

#### Example 2

<img src="/images/melt-pond.png" width="200" style="float:right">
Rapid cross-comparison of multi-sensed regions to enable geo-feature identification and geo-pattern analysis.

<br>

## Ice sheet

Our vast ice sheets are changing rapidly on both regional and continental scales. The recent launch of ICESat-2 also has mission goals to measure ice-sheet surface-change in an effort to quantify the contribution of ice-sheet-mass loss to mean sea level rise. ICESpark will allow users to mine multiple large imagery and high-resolution digital elevation models for seamless GeoBD analysis to answer critical glaciology questions.

<br><br>

## Oceans

Improvements in autonomous ocean observing platforms (e.g., Argo, global surface drifters, seagliders, SailDrones), remote sensing, and an ongoing move towards high-resolution numerical modeling are increasingly transforming oceanography into a big-data science. ICESpark will allow for efficient identification of complementary available observations and provide researchers with significantly faster insight into the interior ocean that is missing in the surface layer remote sensing data.

#### Example

<img src="/images/ocean.png" width="450" style="float:right">
Combine heterogeneous sources to find coincident ocean sensing data off California coast.
