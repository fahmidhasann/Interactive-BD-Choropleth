# Bangladesh Districts Choropleth Map - Educational Data Visualization

## 🌐 **Live Demo**
**🚀 [Check out the interactive map here!](https://fahmidhasann.github.io/Interactive-BD-Choropleth/) 🗺️**

*Try the live version to explore Bangladesh's educational data through interactive choropleth mapping*

---

An interactive web-based choropleth map visualization tool for exploring educational statistics across all 64 districts of Bangladesh. This application provides dynamic data visualization through choropleth mapping with customizable metrics and real-time statistics.

## 🌟 Features

### Interactive Map Visualization
- **Choropleth mapping** of Bangladesh's 64 districts with color-coded data representation
- **Dynamic metric selection** with automatic color scheme assignment
- **Hover interactions** showing detailed district information
- **Click-to-zoom** functionality for focused district exploration
- **Real-time statistics** panel displaying min/max/average values

### Data Management
- **CSV file upload** support for educational metrics
- **GeoJSON file upload** for district boundary data
- **Automatic column detection** from CSV files
- **Multi-version data support** (data v1, v2, v3 with progressive feature additions)
- **Sample datasets included** for testing and demonstration purposes

### Visualization Features
- **Choropleth color coding** with metric-specific palettes
- **Interactive legend** with value ranges
- **Responsive design** for various screen sizes
- **Professional UI** with control panels and info displays

## 🚀 Quick Start

### Prerequisites
- Modern web browser with JavaScript enabled
- CSV file with district education data
- GeoJSON file with Bangladesh district boundaries

### Usage
1. **Open the application**: Launch `map.html` in your web browser
2. **Upload data files**:
   - Select your CSV file containing education metrics
   - Upload the GeoJSON file with district boundaries (`bd_districts.json`)
3. **Load the map**: Click "Load Map Data" button
4. **Explore**: Select different metrics from the control panel to visualize various educational indicators through choropleth mapping

## 📊 Data Structure

### CSV File Format
```csv
district,dropout_rate,student_teacher_ratio,graduation_rate,literacy_rate,womens_education_rate,employment_rate
Dhaka,10.5,24.9,95.86,92.7,93.90981135783018,66.99
Chittagong,19.31,49.2,82.97,88.3,85.95262807032523,88.54
...
```

### Data Versions
- **v1**: Basic metrics (4 columns) - *Sample data for testing*
- **v2**: Extended metrics (5 columns) - *Sample data for testing*
- **v3**: Full metrics including employment data (6 columns) - *Sample data for testing*

> **Note**: All CSV files (data v1.csv, data v2.csv, data v3.csv) contain dummy/sample data for demonstration and testing purposes. Replace with actual educational statistics for production use.

## 🛠️ Technical Architecture

### Frontend Technologies
- **Leaflet.js** - Interactive mapping library for choropleth visualization
- **D3.js** - Data-driven color scaling for choropleth mapping
- **Papa Parse** - CSV file processing
- **Vanilla JavaScript** - Core application logic

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

## 📁 Project Structure
```
bd-district-data-map/
├── map.html              # Main application file
├── bd_districts.json     # GeoJSON district boundaries (to be uploaded)
├── data v1.csv          # Sample education metrics (4 columns)
├── data v2.csv          # Sample education metrics (5 columns)  
├── data v3.csv          # Sample education metrics (6 columns)
└── README.md            # Project documentation
```

> **Important**: The included CSV files contain sample/dummy data for testing the application's functionality. For actual use, replace these with real educational statistics from Bangladesh Bureau of Statistics or other authoritative sources.

## 🔧 Customization

### Adding New Metrics
1. Include new columns in your CSV file
2. The application automatically detects and creates selectors for new metrics
3. Color schemes are intelligently assigned based on metric names

### Modifying Visualizations
- Edit color palettes in the `colorPalettes` array
- Adjust map styling in the CSS section
- Customize tooltips and info panels in the JavaScript functions

## 📈 Data Coverage
- **Geographic Coverage**: All 64 districts of Bangladesh
- **Metric Types**: Educational performance, resource allocation, demographic data
- **Data Quality**: Comprehensive statistics with null value handling
- **Sample Data**: Included CSV files contain dummy data for testing and demonstration

### Data Sources
For production use, obtain real data from:
- Bangladesh Bureau of Statistics (BBS)
- Ministry of Education, Bangladesh
- UNESCO Institute for Statistics
- World Bank Education Statistics

## 🤝 Contributing
Contributions are welcome! Areas for enhancement:
- Additional educational metrics
- Enhanced visualization options
- Performance optimizations
- Mobile responsiveness improvements

## 📄 License
This project is open source and available under the MIT License.

## 🔗 Dependencies
- [Leaflet.js](https://leafletjs.com/) v1.9.4
- [D3.js](https://d3js.org/) v7
- [Papa Parse](https://www.papaparse.com/) v5.4.1
- OpenStreetMap tiles

---
*Built for choropleth map visualization and analysis of Bangladesh's district-level educational statistics.*
