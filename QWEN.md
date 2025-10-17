# Interactive Bangladesh Choropleth Map - Educational Data Visualization

## Overview
An interactive web-based choropleth map visualization tool for exploring educational statistics across all 64 districts of Bangladesh. This application provides dynamic data visualization through choropleth mapping with customizable metrics and real-time statistics. The project allows users to upload their own CSV data files containing educational metrics and GeoJSON files containing district boundary data to visualize the information in an interactive map format.

## Project Structure
```
Interactive-BD-Choropleth/
├── index.html           # Main HTML file implementing the choropleth map interface
├── bangladesh_districts.json # GeoJSON file containing district boundaries for Bangladesh
├── data v1.csv          # Sample CSV data file with 4 educational metrics
├── data v2.csv          # Sample CSV data file with 5 educational metrics
├── data v3.csv          # Sample CSV data file with 6 educational metrics
├── README.md            # Project documentation
└── LICENSE              # MIT License
```

## Features
- Interactive choropleth mapping of Bangladesh's 64 districts with color-coded data representation
- Dynamic metric selection with automatic color scheme assignment
- Hover interactions showing detailed district information
- Click-to-zoom functionality for focused district exploration
- Real-time statistics panel displaying min/max/average values
- CSV file upload support for educational metrics
- GeoJSON file upload support for district boundary data
- Automatic column detection from CSV files
- Responsive design with mobile compatibility
- Professional UI with control panels and info displays

## Data Format
The application accepts CSV files with the following format (sample from data v3.csv):
```
district,dropout_rate,student_teacher_ratio,graduation_rate,literacy_rate,womens_education_rate,employment_rate
Bagerhat,11.43,21.9,86.41,72.5,74.98357076505616,81.11
Bandarban,14.59,27.9,71.6,68.2,67.50867849414408,89.83
...
```

Available sample metrics:
- dropout_rate: Percentage of students who drop out
- student_teacher_ratio: Ratio of students to teachers
- graduation_rate: Percentage of students who graduate
- literacy_rate: Overall literacy rate
- womens_education_rate: Literacy rate for women
- employment_rate: Employment rate in the district

## Technical Architecture
### Frontend Technologies
- **Leaflet.js** - Interactive mapping library for choropleth visualization
- **D3.js** - Data-driven color scaling for choropleth mapping
- **Papa Parse** - CSV file processing
- **Vanilla JavaScript** - Core application logic
- **HTML5/CSS3** - Frontend structure and styling

### Key Components
- **Dynamic Data Loading**: Real-time CSV parsing with column detection
- **Color Scheme Management**: Automatic palette assignment based on metric types
- **Interactive Map Controls**: Zoom, pan, hover, and click interactions
- **Statistics Engine**: Real-time calculation of data summaries

### Browser Compatibility
- Chrome/Chromium 80+
- Firefox 75+
- Safari 13+
- Edge 80+

## Running the Application
1. Simply open `index.html` in a modern web browser
2. Use the file upload controls to upload:
   - A CSV file containing district education data (with 'district' column)
   - A GeoJSON file with district boundaries (the provided `bangladesh_districts.json`)
3. Click the "Load Map Data" button
4. Explore the map by selecting different metrics from the control panel
5. Hover over districts to see detailed information
6. Click on a district to zoom in for more focused viewing

## Customization
### Adding New Metrics
1. Include new columns in your CSV file
2. The application automatically detects and creates selectors for new metrics
3. Color schemes are intelligently assigned based on metric names

### Modifying Visualizations
- Edit color palettes in the `colorPalettes` array in the JavaScript
- Adjust map styling in the CSS section
- Customize tooltips and info panels in the JavaScript functions

## Dependencies
The project relies on the following CDN-hosted libraries:
- Leaflet.js v1.9.4 (https://unpkg.com/leaflet@1.9.4/dist/leaflet.css)
- D3.js v7 (https://d3js.org/d3.v7.min.js)
- Papa Parse v5.4.1 (https://cdnjs.cloudflare.com/ajax/libs/PapaParse/5.4.1/papaparse.min.js)

## Data Sources
For production use, obtain real data from:
- Bangladesh Bureau of Statistics (BBS)
- Ministry of Education, Bangladesh
- UNESCO Institute for Statistics
- World Bank Education Statistics

## License
This project is open source and available under the MIT License.