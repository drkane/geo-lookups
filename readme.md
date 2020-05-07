# geo-lookups

A collection of data resources for handling small-area UK geography.

## [`la_all_codes.csv`](la_all_codes.csv)

A record for each Local Authority that has existed at any time since 2011, with a lookup to the latest Local Authority codes.

Covers England, Northern Ireland, Scotland and Wales.

Fields:

- `LADCD` - Local Authority code
- `LADNM` - Local Authority name
- `LAD20CD` - Local Authority (2020) code
- `LAD20NM` - Local Authority (2020) name
- `UTLACD` - Upper tier local authority code
- `UTLANM` - Upper tier local authority name
- `CAUTHCD` - Combined authority code
- `CAUTHNM` - Combined authority name
- `RGNCD` - Region code
- `RGNNM` - Region name
- `CTRYCD` - Country code
- `CTRYNM` - Country name
- `EWCD` - England and Wales code
- `EWNM` - England and Wales name
- `GBCD` - Great Britain code
- `GBNM` - Great Britain name
- `UKCD` - United Kingdom code
- `UKNM` - United Kingdom name
- `Current` - Whether the LA is currently active

## [`lsoa_la.csv`](lsoa_la.csv)

A record for every Lower Super Output Area from the 2011 census, along with a lookup to the latest Local Authority data.

Covers England, Northern Ireland, Scotland and Wales.Uses "Data Zones" for Scotland and "Super Output Areas" for Northern Ireland.

Fields:

- `LSOA11CD` - Lower Super Output Area code
- `LSOA11NM` - Lower Super Output Area name
- `MSOA11CD` - Middle Super Output Area code
- `MSOA11NM` - Middle Super Output Area name
- `MSOA11HCLNM` - Middle Super Output Area name from [House of Commons Library](https://visual.parliament.uk/msoanames)
- `LAD17CD` - Local Authority (2017) code
- `LAD20CD` - Local Authority (2020) code
- `LAD20NM` - Local Authority (2020) name
- `UTLACD` - Upper tier local authority code
- `UTLANM` - Upper tier local authority name
- `CAUTHCD` - Combined authority code
- `CAUTHNM` - Combined authority name
- `RGNCD` - Region code
- `RGNNM` - Region name
- `CTRYCD` - Country code
- `CTRYNM` - Country name
- `EWCD` - England and Wales code
- `EWNM` - England and Wales name
- `GBCD` - Great Britain code
- `GBNM` - Great Britain name
- `UKCD` - United Kingdom code
- `UKNM` - United Kingdom name

## [`lsoa_latlong.csv`](lsoa_latlong.csv)

A record for every Lower Super Output Area from the 2011 census, along with the latitude and longitude of the centre of the area.

Covers England, Northern Ireland, Scotland and Wales.Uses "Data Zones" for Scotland and "Super Output Areas" for Northern Ireland. For England and Wales the latitude and longitude centers are population-weighted.

Fields:

- `lsoa11cd` - Lower Super Output Area code
- `longitude` - Longitude of central point
- `latitude` - Latitude of central point

## [`msoa_la.csv`](msoa_la.csv)

A record for every Middle Super Output Area from the 2011 census, along with a lookup to the latest Local Authority data.

Covers England, Northern Ireland, Scotland and Wales. Uses "Intermediate Zones" for Scotland and "Super Output Areas" for Northern Ireland.

Fields:

- `MSOA11CD` - Middle Super Output Area code
- `MSOA11NM` - Middle Super Output Area name
- `MSOA11HCLNM` - Middle Super Output Area name from [House of Commons Library](https://visual.parliament.uk/msoanames)
- `LAD17CD` - Local Authority (2017) code
- `LAD20CD` - Local Authority (2020) code
- `LAD20NM` - Local Authority (2020) name
- `UTLACD` - Upper tier local authority code
- `UTLANM` - Upper tier local authority name
- `CAUTHCD` - Combined authority code
- `CAUTHNM` - Combined authority name
- `RGNCD` - Region code
- `RGNNM` - Region name
- `CTRYCD` - Country code
- `CTRYNM` - Country name
- `EWCD` - England and Wales code
- `EWNM` - England and Wales name
- `GBCD` - Great Britain code
- `GBNM` - Great Britain name
- `UKCD` - United Kingdom code
- `UKNM` - United Kingdom name

## [`msoa_latlong.csv`](msoa_latlong.csv)

A record for every Middle Super Output Area from the 2011 census, along with the latitude and longitude of the centre of the area.

Covers England, Northern Ireland, Scotland and Wales.Uses "Intermediate Zones" for Scotland and "Super Output Areas" for Northern Ireland. For England and Wales the latitude and longitude centers are population-weighted.

Fields:

- `msoa11cd` - Lower Super Output Area code
- `longitude` - Longitude of central point
- `latitude` - Latitude of central point

## [`ward_all_codes.csv`](ward_all_codes.csv)

A record for every Ward in the UK that has existed since 2015, along with a lookup to the latest Local Authority that it would be part of. Lookups are based on a lookup from the Local Authority that the ward belonged to at the time it existed to the latest Local Authorities. So these could be incorrect in a few cases.

Covers England, Northern Ireland, Scotland and Wales.

Fields:

- `WDCD` - Middle Super Output Area code
- `WDNM` - Middle Super Output Area name
- `LADCD` - Local Authority code from source data
- `LADNM` - Local Authority name from source data
- `SOURCEFILE` - Source year for the ward data
- `LAD17CD` - Local Authority (2017) code
- `LAD20CD` - Local Authority (2020) code
- `LAD20NM` - Local Authority (2020) name
- `UTLACD` - Upper tier local authority code
- `UTLANM` - Upper tier local authority name
- `CAUTHCD` - Combined authority code
- `CAUTHNM` - Combined authority name
- `RGNCD` - Region code
- `RGNNM` - Region name
- `CTRYCD` - Country code
- `CTRYNM` - Country name
- `EWCD` - England and Wales code
- `EWNM` - England and Wales name
- `GBCD` - Great Britain code
- `GBNM` - Great Britain name
- `UKCD` - United Kingdom code
- `UKNM` - United Kingdom name

## [`ward_latlong.csv`](ward_latlong.csv)

A record for every Ward in the UK that has existed since 2015, along with the latitude and longitude of the centre of the area.

Covers England, Northern Ireland, Scotland and Wales.

Fields:

- `wdcd` - Ward code
- `longitude` - Longitude of central point
- `latitude` - Latitude of central point

## Data sources

Data is sourced from the [ONS Geoportal](http://geoportal.statistics.gov.uk/) and used under the Open Government Licence v3.0. 

Other data sources:

- [Scottish Data Zone Centroids](https://data.gov.uk/dataset/8aabd120-6e15-41bf-be7c-2536cbc4b2e5/data-zone-centroids-2011)
- [Scottish Intermediate Zone Centroids](https://data.gov.uk/dataset/df24c284-f34d-4a2f-88fe-27e3a3b9ac90/intermediate-zone-centroids-2011)
- [House of Commons Library MSOA names](https://visual.parliament.uk/msoanames)
- [Northern Ireland Super Output Areas](https://www.nisra.gov.uk/support/geography/northern-ireland-super-output-areas)
