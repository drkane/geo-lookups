# geo-lookups

A collection of data resources for handling small-area UK geography.

## [Boundary files](boundaries/)

A collection of geojson files for local authorities that give the boundaries of wards, LSOAs and MSOAs within that authority.

- [`boundaries/`](boundaries/)

## [`la_all_codes.csv`](la_all_codes.csv)

A record for each Lower Tier Local Authority that has existed at any time since 2011, with a lookup to the latest Local Authority codes.

Covers England, Northern Ireland, Scotland and Wales.

Fields:

- `LADCD` - Local Authority code (includes areas that are no longer active)
- `LADNM` - Local Authority name (includes areas that are no longer active)
- `LADCD_ACTIVE` - Local Authority code (the most recent code that covers this area)
- `LADNM_ACTIVE` - Local Authority name (the most recent name that covers this area)
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

The following columns are included for compatability but are deprecated
and can expected to be removed in future versions:

- `LAD20CD` - Local Authority (2020) code
- `LAD20NM` - Local Authority (2020) name

## [`utla_all_codes.csv`](utla_all_codes.csv)

A record for each Upper Tier Local Authority.

Covers England, Northern Ireland, Scotland and Wales.

Fields:

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

## [`lsoa_la.csv`](lsoa_la.csv)

A record for every Lower Super Output Area from the 2011 and 2021 censuses, along with a lookup to the latest Local Authority data.

Covers England, Northern Ireland, Scotland and Wales. Uses "Data Zones" for Scotland (2011 census only). For Northern Ireland the file includes "Super Output Areas" for the 2011 Census and "Data Zones" for the 2021 Census.

Fields:

- `LSOACD` - Lower Super Output Area code
- `LSOANM` - Lower Super Output Area name
- `MSOACD` - Middle Super Output Area code
- `MSOANM` - Middle Super Output Area name
- `MSOAHCLNM` - Middle Super Output Area name in English from [House of Commons Library](https://visual.parliament.uk/msoanames)
- `MSOAHCLNMW` - Middle Super Output Area name in Welsh from [House of Commons Library](https://visual.parliament.uk/msoanames)
- `LADCD_ACTIVE` - Local Authority code (the most recent code that covers this area)
- `LADNM_ACTIVE` - Local Authority name (the most recent name that covers this area)
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
- `LSOA11CD` - Lower Super Output Area code (if code existed in 2011 Census)
- `LSOA21CD` - Lower Super Output Area code (if code existed in 2021 Census)

The following columns are included for compatability but are deprecated
and can expected to be removed in future versions:

- `LAD17CD` - Local Authority (2017) code
- `LAD20CD` - Local Authority (2020) code
- `LAD20NM` - Local Authority (2020) name
- `LSOA11NM` - Lower Super Output Area code
- `MSOA11CD` - Middle Super Output Area code
- `MSOA11NM` - Middle Super Output Area name
- `MSOA11HCLNM` - Middle Super Output Area name from [House of Commons Library](https://visual.parliament.uk/msoanames)
- `TTWA11CD` - Travel to work area code
- `TTWA11NM` - Travel to work area name

## [`lsoa_latlong.csv`](lsoa_latlong.csv)

A record for every Lower Super Output Area from the 2011 and 2021 censuses, along with the latitude and longitude of the centre of the area.

Covers England, Northern Ireland, Scotland and Wales. Uses "Data Zones" for Scotland (2011 census only). For Northern Ireland the file includes "Super Output Areas" for the 2011 Census and "Data Zones" for the 2021 Census.

Fields:

- `LSOACD` - Lower Super Output Area code
- `longitude` - Longitude of central point
- `latitude` - Latitude of central point

The following columns are included for compatability but are deprecated
and can expected to be removed in future versions:

- `lsoa11cd` - Lower Super Output Area code

## [`msoa_la.csv`](msoa_la.csv)

A record for every Middle Super Output Area from the 2011 and 2021 censuses, along with a lookup to the latest Local Authority data.

Covers England, Northern Ireland, Scotland and Wales. Uses "Intermediate Zones" for Scotland (2011 census only). For Northern Ireland the file includes "Super Output Areas" for the 2011 Census and "Super Data Zones" for the 2021 Census.

Fields:

- `MSOACD` - Middle Super Output Area code
- `MSOANM` - Middle Super Output Area name
- `MSOAHCLNM` - Middle Super Output Area name in English from [House of Commons Library](https://visual.parliament.uk/msoanames)
- `MSOAHCLNMW` - Middle Super Output Area name in Welsh from [House of Commons Library](https://visual.parliament.uk/msoanames)
- `LADCD_ACTIVE` - Local Authority code (the most recent code that covers this area)
- `LADNM_ACTIVE` - Local Authority name (the most recent name that covers this area)
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
- `MSOA11CD` - Middle Super Output Area code (if code existed in 2011 Census)
- `MSOA21CD` - Middle Super Output Area code (if code existed in 2021 Census)

The following columns are included for compatability but are deprecated
and can expected to be removed in future versions:

- `LAD17CD` - Local Authority (2017) code
- `LAD20CD` - Local Authority (2020) code
- `LAD20NM` - Local Authority (2020) name
- `MSOA11NM` - Middle Super Output Area name
- `MSOA11HCLNM` - Middle Super Output Area name from [House of Commons Library](https://visual.parliament.uk/msoanames)

## [`msoa_latlong.csv`](msoa_latlong.csv)

A record for every Middle Super Output Area from the 2011 and 2021 censuses, along with the latitude and longitude of the centre of the area.

Covers England, Northern Ireland, Scotland and Wales. Uses "Intermediate Zones" for Scotland (2011 census only). For Northern Ireland the file includes "Super Output Areas" for the 2011 Census and "Super Data Zones" for the 2021 Census.

Fields:

- `MSOACD` - Middle Super Output Area code
- `longitude` - Longitude of central point
- `latitude` - Latitude of central point

The following columns are included for compatability but are deprecated
and can expected to be removed in future versions:

- `msoa11cd` - Middle Super Output Area code

## [`ward_all_codes.csv`](ward_all_codes.csv)

A record for every Ward in the UK that has existed since 2015, along with a lookup to the latest Local Authority that it would be part of. Lookups are based on a lookup from the Local Authority that the ward belonged to at the time it existed to the latest Local Authorities. So these could be incorrect in a few cases.

Covers England, Northern Ireland, Scotland and Wales.

Fields:

- `WDCD` - Ward code
- `WDNM` - Ward name
- `LADCD` - Local Authority code from source data
- `LADNM` - Local Authority name from source data
- `SOURCEFILE` - Source year for the ward data
- `LAD17CD` - Local Authority (2017) code
- `LADCD_ACTIVE` - Local Authority code (the most recent code that covers this area)
- `LADNM_ACTIVE` - Local Authority name (the most recent name that covers this area)
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

The following columns are included for compatability but are deprecated
and can expected to be removed in future versions:

- `LAD20CD` - Local Authority (2020) code
- `LAD20NM` - Local Authority (2020) name

## [`ward_latlong.csv`](ward_latlong.csv)

A record for every Ward in the UK that has existed since 2015, along with the latitude and longitude of the centre of the area.

Covers England, Northern Ireland, Scotland and Wales.

Fields:

- `wdcd` - Ward code
- `longitude` - Longitude of central point
- `latitude` - Latitude of central point

## [`cauth_all_codes.csv`](cauth_all_codes.csv)

A record for each Combined Authority.

Covers England

Fields:

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

## [`rgn_all_codes.csv`](rgn_all_codes.csv)

A record for each English region.

Covers England

Fields:

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

## [`ctry_all_codes.csv`](ctry_all_codes.csv)

A record for each Country.

Covers England, Northern Ireland, Scotland and Wales.

Fields:

- `CTRYCD` - Country code
- `CTRYNM` - Country name
- `EWCD` - England and Wales code
- `EWNM` - England and Wales name
- `GBCD` - Great Britain code
- `GBNM` - Great Britain name
- `UKCD` - United Kingdom code
- `UKNM` - United Kingdom name

The following files are also created for completeness, although they only include one record each.

- [`ew_all_codes.csv`](ew_all_codes.csv)
- [`gb_all_codes.csv`](gb_all_codes.csv)
- [`uk_all_codes.csv`](uk_all_codes.csv)

## [`la_orgid_to_gss.csv`](la_orgid_to_gss.csv)

A lookup between the codes for Local Authorities from the (now defunct) registers of
Local Authorities held by gov.uk with the GSS codes for the areas they represent.

Fields:


- `org_id` - Council identifier
- `name` - Name of the Council
- `normalised_name` - Area name standardised
- `gss_code` - GSS Code for the area
- `area_name` - Name of the area from GSS record
- `area_type` - Entity type of the area
- `active` - Whether it's a currently active area

## [`area_all_codes.csv`](area_all_codes.csv)

Based on `la_all_codes.csv`, this file also adds records for administrative geography at a higher level than local authority districts, so there are records for:
 - upper tier local authorities
 - combined authorities
 - regions
 - countries (including "England and Wales", "Great Britain" and "United Kingdom" as separate codes)

Each record contains links to areas that can be inferred from the given code. Where defunct local authorities are included, their record links to the most up to date code for that authority.

Fields:

- `areacode` - GSS code for the area
- `areaname` - Name for the area
- `areatype` - Type of area. One of (`la`, `utla`, `cauth`, `rgn`, `ctry`, `ew`, `gb`, `uk`)
- `LADCD` - Local Authority code (the most recent code that covers this area)
- `LADNM` - Local Authority name (the most recent name that covers this area)
- `LADCD_ACTIVE` - Local Authority code (the most recent code that covers this area - duplicate with `LADCD` but included for completeness and compatability)
- `LADNM_ACTIVE` - Local Authority name (the most recent name that covers this area - duplicate with `LADNM` but included for completeness and compatability)
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

## Other files

### [`lieutenancy_areas_england.csv`](misc/lieutenancy_areas_england.csv)

A list of the [lieutenancy areas of England](https://en.wikipedia.org/wiki/Ceremonial_counties_of_England#Lieutenancy_areas_since_1997) from 1997, based on data from Wikidata and Wikipedia, mapped to current and former local authority codes. These are sometimes known as ceremonial counties.

Note that according to Wikipedia the local authority areas have a 1:1 match with the boundaries of ceremonial areas, with the exception of Stockton-on-Tees (`E06000004`) which is shared between County Durham (north of the Tees) and North Yorkshire (south of the Tees). For the purposes of this list Stockton-on-Tees has been allocated to County Durham, but this is not completely accurate.

- `LADCD` - Local Authority code (includes areas that are no longer active)
- `LADNM` - Local Authority name (includes areas that are no longer active)
- `LADCD_ACTIVE` - Local Authority code (the most recent code that covers this area)
- `LADNM_ACTIVE` - Local Authority name (the most recent name that covers this area)
- `UTLACD` - Upper tier local authority code
- `UTLANM` - Upper tier local authority name
- `LIEUTENANCY_AREA_1997` - The name of the Lieutenancy Area as defined by the Lieutenancies Act 1997
- `LIEUTENANCY_AREA_1997_WIKIDATA` - Wikidata code for the Lieutenancy Area

## Data sources

Data is sourced from the [ONS Geoportal](http://geoportal.statistics.gov.uk/) and used under the Open Government Licence v3.0. 

Other data sources:

- [Scottish Data Zone Centroids](https://data.gov.uk/dataset/8aabd120-6e15-41bf-be7c-2536cbc4b2e5/data-zone-centroids-2011)
- [Scottish Intermediate Zone Centroids](https://data.gov.uk/dataset/df24c284-f34d-4a2f-88fe-27e3a3b9ac90/intermediate-zone-centroids-2011)
- [House of Commons Library MSOA names](https://visual.parliament.uk/msoanames)
- [Northern Ireland Super Output Areas](https://www.nisra.gov.uk/support/geography/northern-ireland-super-output-areas)
