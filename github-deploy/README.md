# Interactive Iberian Songs Platform 🎵

[![Live Demo](https://img.shields.io/badge/Live%20Demo-GitHub%20Pages-blue)](https://YOUR_USERNAME.github.io/iberian-songs-map)
[![Songs](https://img.shields.io/badge/Songs-801-green)](https://YOUR_USERNAME.github.io/iberian-songs-map)
[![Themes](https://img.shields.io/badge/Themes-6-orange)](https://YOUR_USERNAME.github.io/iberian-songs-map)

An interactive digital platform for exploring traditional Spanish and Portuguese songs through an innovative geographical and thematic interface.

## 🌟 Features

- **Interactive Map**: Explore 801 traditional songs mapped to their geographic origins
- **Thematic Filtering**: Discover songs by 6 thematic categories (Affect & Desires, Family, Religious, Natural Imagery, Ritual, Symbolic Traditional)
- **Audio Playback**: Listen to MIDI interpretations of historical musical notation
- **Educational Tools**: Difficulty analysis and cultural context for each song
- **Mobile Responsive**: Works seamlessly on desktop, tablet, and mobile devices

## 📊 Collection Overview

| Country | Songs | Regions | With Geolocation |
|---------|-------|---------|------------------|
| Spain | 742 | 17 regions | 641 (86.4%) |
| Portugal | 59 | 5 regions | 59 (100%) |
| **Total** | **801** | **22 regions** | **700 (87.4%)** |

## 🎓 Educational Applications

This platform serves multiple educational contexts:
- **K-12 Education**: Cultural geography, music history, language learning
- **Higher Education**: Ethnomusicology, digital humanities, cultural studies
- **Research**: Academic analysis of traditional music patterns and distributions
- **Cultural Heritage**: Preservation and dissemination of Iberian musical traditions

## 🗺️ Geographic Coverage

### Spanish Regions
Andalucía, Aragón, Asturias, Cantabria, Castilla-La Mancha, Castilla y León, Cataluña, Comunidad de Madrid, Comunidad Valenciana, Extremadura, Galicia, Islas Baleares, Islas Canarias, La Rioja, Navarra, País Vasco, Región de Murcia

### Portuguese Regions
Braga, Faro, Viana do Castelo, Vila Real, and additional regional classifications

## 🏷️ Thematic Categories

1. **Affect & Desires** (160 songs) - Emotions, love, personal relationships
2. **Family** (143 songs) - Family relationships, domestic life
3. **Honorific - Religious** (105 songs) - Religious themes, spiritual content
4. **Natural Imagery** (95 songs) - Nature, landscapes, seasonal themes
5. **Ritual** (85 songs) - Ceremonial and traditional practices
6. **Symbolic Traditional** (75 songs) - Cultural symbols and traditions

## 🔧 Technology Stack

- **Frontend**: HTML5, CSS3, JavaScript (ES6+)
- **Mapping**: Leaflet.js with custom geographic boundaries
- **Audio**: Web Audio API for MIDI playback
- **Data Format**: MEI (Music Encoding Initiative) for musical notation
- **Hosting**: GitHub Pages (static site hosting)

## 📚 Academic Documentation

- [Educational Applications Analysis](Academic_Chapter_Interactive_Cultural_Heritage_Platform.md)
- [Data Architecture Analysis](Academic_Chapter_Data_Analysis.md)
- [Geolocation Validation Report](GEOLOCATION_VALIDATION_REPORT.md)
- [Filter Distribution Analysis](FILTER_DISTRIBUTION_ANALYSIS.md)

## 🚀 Quick Start

1. **Visit the live platform**: [YOUR_USERNAME.github.io/iberian-songs-map](https://YOUR_USERNAME.github.io/iberian-songs-map)
2. **Explore the map**: Click on regions to see available songs
3. **Filter by themes**: Use the thematic filter dropdown
4. **Play songs**: Click on song markers to hear MIDI playback
5. **Learn more**: Access song metadata and cultural context

## 📖 Usage

### For Educators
- Use as a teaching tool for cultural geography
- Demonstrate the relationship between geography and musical traditions
- Assign research projects based on regional or thematic exploration

### For Researchers
- Access comprehensive metadata for each song
- Analyze patterns in musical distribution across regions
- Export data for further academic analysis

### For Students
- Explore cultural heritage through interactive engagement
- Develop understanding of Iberian musical traditions
- Practice language skills with traditional lyrics

## 🛠️ Development

### Local Development
```bash
# Clone the repository
git clone https://github.com/YOUR_USERNAME/iberian-songs-map.git
cd iberian-songs-map

# Start local server
python3 -m http.server 8000

# Open browser
open http://localhost:8000
```

### Data Structure
- `Spanish/`: 742 MEI files containing Spanish traditional songs
- `Portuguese/`: 59 MEI files containing Portuguese traditional songs
- `thematic_map.json`: Thematic classifications for songs
- `spanish-mei-location-mapping.json`: Geographic mappings for Spanish songs
- `portuguese-mei-location-mapping.json`: Geographic mappings for Portuguese songs
- `song_difficulty_analysis.json`: Educational difficulty assessments

## 📄 Data Sources

- **Musical Notation**: Traditional songs encoded in MEI format
- **Geographic Data**: Regional boundaries and cultural geographic classifications
- **Thematic Analysis**: Academic clustering analysis of lyrical content
- **Cultural Context**: Historical and ethnomusicological research

## 🤝 Contributing

This project welcomes contributions from:
- **Ethnomusicologists**: Additional song analysis and cultural context
- **Educators**: Pedagogical improvements and educational features
- **Developers**: Technical enhancements and new functionality
- **Cultural Heritage Experts**: Data validation and expansion

## 📧 Contact

For academic collaboration, data requests, or technical support, please create an issue in this repository.

## 📜 License

This project is designed for educational and research purposes. Please respect the cultural heritage nature of the traditional songs and use appropriate attribution in academic work.

## 🙏 Acknowledgments

- Traditional music collectors and ethnomusicologists who preserved these cultural treasures
- The MEI (Music Encoding Initiative) community for providing standards for digital music representation
- Open source mapping and web audio communities for enabling this interactive platform

---

**Explore the rich musical heritage of the Iberian Peninsula through this innovative digital platform combining geography, culture, and technology.**
