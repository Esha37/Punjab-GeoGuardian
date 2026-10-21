
# Punjab GeoGuardian

## AI-Based Monitoring of Urban Expansion and Farmland Loss

Punjab GeoGuardian is an educational GeoAI prototype that uses Sentinel-2 satellite imagery and machine learning to analyze possible land-use changes in Faisalabad District, Punjab, Pakistan.

The project compares satellite imagery from 2019 and 2025 and identifies possible changes from vegetation/agricultural land to built-up/urban land.

## Project Area

- Area of Interest: Faisalabad District
- Province: Punjab, Pakistan
- Total AOI area: 5953.79 km2
- Years compared: 2019 and 2025

## Main Objectives

- Analyze vegetation and agricultural land
- Detect built-up and urban areas
- Calculate NDVI and NDBI
- Apply Random Forest classification
- Detect possible vegetation-to-built-up conversion
- Calculate approximate area statistics
- Validate the classification using manually checked points
- Create an interactive map dashboard

## Data and Tools

- Google Colab
- Google Earth Engine
- Sentinel-2 Surface Reflectance Harmonized
- Python
- Geemap
- Folium
- Pandas
- NumPy
- Scikit-learn
- Random Forest

## Land-Cover Classes

| Class ID | Class |
|---:|---|
| 0 | Other |
| 1 | Vegetation / Agriculture |
| 2 | Built-up / Urban |

## Remote-Sensing Indices

### NDVI

NDVI was used to identify vegetation and agricultural areas.

NDVI = (NIR - Red) / (NIR + Red)

### NDBI

NDBI was used to support built-up and urban-area identification.

NDBI = (SWIR - NIR) / (SWIR + NIR)

## Results

| Metric | Value |
|---|---:|
| Total AOI area | 5953.79 km2 |
| Vegetation / Agriculture area in 2019 | 4643.94 km2 |
| Built-up / Urban area in 2025 | 838.99 km2 |
| Estimated vegetation-to-built-up conversion | 344.84 km2 |
| Percentage of AOI affected | 5.79% |
| Validation points | 60 |
| Validation accuracy | 96.67% |

## Important Interpretation

The estimated vegetation-to-built-up conversion represents pixels classified as vegetation or agriculture in 2019 and built-up or urban in 2025.

These results are estimated satellite-based outputs. They should not be treated as official land records, legal evidence, or an official government monitoring system.

## Project Outputs

- Punjab GeoGuardian Google Colab notebook
- RGB maps for 2019 and 2025
- NDVI maps for 2019 and 2025
- NDBI maps for 2019 and 2025
- Land classification maps
- Vegetation-to-built-up change map
- Area statistics tables
- Validation results
- Error-analysis file
- Interactive HTML dashboard
- Final project report

## Limitations

- Sentinel-2 imagery has a spatial resolution of approximately 10 metres for key bands.
- Mixed pixels may cause classification errors.
- Dry soil can be confused with built-up land.
- Seasonal crop changes may affect NDVI.
- Small buildings and narrow roads may not be detected.
- Image dates and atmospheric conditions may differ.
- More manually verified training and validation samples would improve reliability.

## Future Improvements

- Add more land-cover classes
- Use higher-resolution imagery
- Compare multiple years
- Add district-level monitoring
- Use official reference datasets
- Test segmentation models such as U-Net
- Build a Streamlit dashboard
- Add automated PDF reporting

## Disclaimer

This project was developed for educational and internship purposes. It is a learning prototype and is not an official government monitoring or decision-support system.
