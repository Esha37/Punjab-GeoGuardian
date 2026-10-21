
# Punjab GeoGuardian Final Report

## Project

Punjab GeoGuardian is an educational GeoAI prototype for monitoring possible
urban expansion and farmland loss in Faisalabad District, Punjab, Pakistan.

## Data and Method

The project compares Sentinel-2 satellite imagery from 2019 and 2025.
Cloud-masked median composites were created using Google Earth Engine.
NDVI and NDBI were calculated, followed by Random Forest land-cover
classification.

The classes are:

- Other
- Vegetation / Agriculture
- Built-up / Urban

Possible conversion is defined as pixels classified as vegetation/agriculture
in 2019 and built-up/urban in 2025.

## Results

- Total AOI area: 5,953.79 km2
- Vegetation/agriculture area in 2019: 4,643.94 km2
- Built-up/urban area in 2025: 838.99 km2
- Estimated vegetation-to-built-up conversion: 344.84 km2
- Estimated AOI affected: 5.79%
- Validation points: 60
- Validation accuracy: 96.67%

## Limitations

The results are estimates. Dry soil, seasonal crop changes, mixed pixels,
small buildings, image dates, cloud masking, and training-label quality can
affect classification accuracy.

## Disclaimer

This project is an educational learning prototype. It is not an official
government monitoring system, legal land record, or official decision-making
system.
