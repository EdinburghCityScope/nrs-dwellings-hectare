# nrs-dwellings-hectare
Number of dwellings per hectare in Edinburgh.

Data on number of dwellings is obtained from the Assessors’ Portal. The Assessors are, amongst other things, responsible for valuing each dwelling in Scotland for the purposes of assigning it to a Council Tax Band.

Dwellings - This is the total number of dwellings on the Council Tax valuation list (excluding free-standing private lock-ups and garages). A 'dwelling' refers to the accommodation itself, for example a house or a flat, and includes second homes that are not let out commercially. Caravans count as dwellings if they are someone’s main home.

Dwellings per hectare - This variable has been calculated by dividing the total number of dwellings by the area in hectares, as determined by a NRS in-house measure.

Summary statistics on dwellings in Scotland are published annually in 'Estimates of Households and Dwellings in Scotland', which is available on the [NRS website](http://www.nrscotland.gov.uk/statistics-and-data/statistics/statistics-by-theme/housholds/household-estimates).

Statistics provided by National Records of Scotland:  http://statistics.gov.scot/data/dwellings-hectare

## License

Data is licensed under the Open Government License: http://www.nationalarchives.gov.uk/doc/open-government-licence/version/2/

## Requirements

- NodeJS
- npm

## Installation

Clone the repository

```
git clone https://github.com/EdinburghCityScope/nrs-dwellings-hectare.git
```

Install npm dependencies

```
cd nrs-dwellings-hectare
npm install
```

Run the API (from the nrs-dwellings-hectare directory)

```
node .
```

Converting the extracted data into loopback data.

```
node scripts/featureCollectionToLoopbackJson.js
```

Re-build data files from the statistics.gov.scot API

```
node scripts/build-data.js
```
