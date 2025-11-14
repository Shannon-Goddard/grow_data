# 🌿 Grow Data - Cannabis Strain Database

> **Comprehensive Cannabis Strain Dataset | 2,793+ Strains | Web Scraping & Data Processing**

[![MIT License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)
[![Python](https://img.shields.io/badge/Python-3.7+-blue.svg)](https://python.org)
[![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange.svg)](https://jupyter.org)
[![Data Source](https://img.shields.io/badge/Data_Source-Wikileaf-purple.svg)](https://www.wikileaf.com/strains/)

## 🚀 Project Overview

**Grow Data** is a comprehensive cannabis strain database containing detailed information on **2,793 unique cannabis strains** scraped from Wikileaf.com. This project demonstrates advanced web scraping techniques, data cleaning, and processing methodologies to create a structured dataset for cannabis research and application development.

### 🎯 Key Features

- **2,793+ Cannabis Strains** with complete profiles
- **Comprehensive Data Points** including THC/CBD levels, strain types, effects, and descriptions
- **Clean, Structured Data** in multiple formats (CSV, JSON, JavaScript)
- **Web Scraping Pipeline** using Python, Pandas, and Beautiful Soup
- **Data Processing Notebooks** for cleaning and transformation
- **Ready-to-Use Datasets** for web applications and research

## 📊 Dataset Statistics

| Metric | Value |
|--------|-------|
| **Total Strains** | 2,793 |
| **Data Points per Strain** | 8+ fields |
| **File Formats** | CSV, JSON, JavaScript |
| **Data Source** | Wikileaf.com |
| **Processing Method** | Python + Beautiful Soup |

## 🗂️ Data Structure

Each strain record contains:

```javascript
{
  index: "0",
  strain: "Green Crack",
  strain_url: "https://www.wikileaf.com/strain/green-crack/",
  logo: "https://assets.wikileaf.com/assets/strains/strain/...",
  info: "<p>Detailed strain information...</p>",
  more_info: "<p>Additional strain details...</p>",
  THC: "<p>THC level classification</p>",
  CBD: "<p>CBD level classification</p>",
  Sativa: "<p>Sativa percentage</p>",
  Indica: "<p>Indica percentage</p>"
}
```

## 📁 Project Structure

```
grow_data/
├── Resources/
│   ├── csv/                    # Processed CSV datasets
│   │   ├── ALL_data.csv       # Complete strain database
│   │   ├── strain_data.csv    # Strain names and URLs
│   │   ├── logo_data.csv      # Strain logos and images
│   │   └── more_info_data.csv # Extended strain information
│   ├── js/                    # JavaScript data and notebooks
│   │   ├── data.js           # JavaScript-formatted dataset
│   │   ├── ALL_data.ipynb    # Main data processing notebook
│   │   ├── TableBuild_*.ipynb # Specialized processing notebooks
│   │   └── about_strain.ipynb # Strain analysis notebook
│   └── pics/                  # Project assets
│       ├── header_pic.png    # Project header image
│       └── gif.gif          # Demo animation
├── LICENSE                    # MIT License
└── README.md                 # This file
```

## 🛠️ Technologies Used

- **Python 3.7+** - Core programming language
- **Pandas** - Data manipulation and analysis
- **Beautiful Soup** - Web scraping and HTML parsing
- **Jupyter Notebook** - Interactive development environment
- **CSV/JSON** - Data storage formats
- **JavaScript** - Client-side data integration

## 🚀 Getting Started

### Prerequisites

```bash
pip install pandas beautifulsoup4 requests jupyter
```

### Quick Start

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/grow_data.git
   cd grow_data
   ```

2. **Explore the data**
   ```python
   import pandas as pd
   
   # Load the complete dataset
   df = pd.read_csv('Resources/csv/ALL_data.csv')
   print(f"Total strains: {len(df)}")
   print(df.head())
   ```

3. **Use in web applications**
   ```html
   <script src="Resources/js/data.js"></script>
   <script>
     console.log(`Loaded ${strainData.length} strains`);
   </script>
   ```

## 📈 Data Processing Pipeline

### 1. Web Scraping
- **Target**: Wikileaf.com strain database
- **Method**: Beautiful Soup + Requests
- **Scope**: 2,793+ individual strain pages

### 2. Data Cleaning
- **HTML Processing**: Extract clean text from HTML content
- **Data Validation**: Ensure data integrity and consistency
- **Error Handling**: Manage missing data and scraping failures

### 3. Data Transformation
- **Format Conversion**: CSV → JSON → JavaScript
- **Structure Optimization**: Organize for different use cases
- **Performance**: Optimize for web application loading

## 🎯 Use Cases

### 🔬 Research Applications
- Cannabis strain analysis and classification
- THC/CBD distribution studies
- Strain effect correlation research
- Market trend analysis

### 💻 Web Development
- Cannabis strain search engines
- Grow planning applications
- Educational platforms
- E-commerce integration

### 📊 Data Science
- Machine learning model training
- Natural language processing on strain descriptions
- Recommendation system development
- Market analysis and insights

## 📋 Data Fields

| Field | Description | Type |
|-------|-------------|------|
| `index` | Unique strain identifier | Integer |
| `strain` | Strain name | String |
| `strain_url` | Wikileaf strain page URL | URL |
| `logo` | Strain image URL | URL |
| `info` | Primary strain description | HTML/Text |
| `more_info` | Additional strain details | HTML/Text |
| `THC` | THC level classification | String |
| `CBD` | CBD level classification | String |
| `Sativa` | Sativa percentage indicator | String |
| `Indica` | Indica percentage indicator | String |

## 🔍 Sample Data

```csv
index,strain,THC,CBD,Sativa,Indica
0,Green Crack,Normal,Very Low,Normal,Very Low
1,Blue Dream,Very High,Very Low,Very High,Very Low
2,Sour Diesel,Very High,Very Low,Very High,Very Low
```

## 🤝 Contributing

We welcome contributions to improve the dataset and processing pipeline!

### How to Contribute

1. **Fork** the repository
2. **Create** a feature branch (`git checkout -b feature/enhancement`)
3. **Commit** your changes (`git commit -m 'Add enhancement'`)
4. **Push** to the branch (`git push origin feature/enhancement`)
5. **Open** a Pull Request

### Areas for Contribution

- 🔄 **Data Updates** - Refresh strain information
- 🧹 **Data Cleaning** - Improve processing algorithms
- 📊 **Analysis Tools** - Add data analysis notebooks
- 🌐 **Integration** - Create API endpoints
- 📚 **Documentation** - Enhance guides and examples

## ⚠️ Limitations & Considerations

- **Data Currency**: Scraped data reflects Wikileaf content at time of collection
- **Manual Intervention**: Some strain names required manual correction due to URL inconsistencies
- **Legal Compliance**: Ensure compliance with local cannabis laws when using this data
- **Attribution**: Data sourced from Wikileaf.com - respect their terms of service

## 🔗 Related Projects

This dataset powers several applications in the cannabis cultivation ecosystem:

- **[GrowApp Cannabis Guide](https://growappcannabis.guide)** - Comprehensive grow planning platform
- **Strain Search Tools** - Advanced strain discovery interfaces
- **Nutrient Calculators** - Feeding schedule generators
- **Plant Diagnostics** - Problem identification systems

## 📄 License

This project is licensed under the **MIT License** - see the [LICENSE](LICENSE) file for details.

### License Summary
- ✅ **Commercial use** allowed
- ✅ **Modification** allowed  
- ✅ **Distribution** allowed
- ✅ **Private use** allowed
- ❗ **License and copyright notice** required

## 🙏 Acknowledgments

- **Wikileaf.com** - Primary data source for strain information
- **Cannabis Community** - For strain knowledge and cultivation wisdom
- **Open Source Contributors** - For tools and libraries that made this possible
- **Python Community** - For Beautiful Soup, Pandas, and Jupyter ecosystems

## 📞 Contact & Support

- **Issues**: [GitHub Issues](https://github.com/Shannon-Goddard/grow_data/issues)
- **Discussions**: [GitHub Discussions](https://github.com/Shannon-Goddard/grow_data/discussions)
- **Email**: shannon@loyal9.app

---

<div align="center">

**Built with 🌿 for the cannabis cultivation community**

*Empowering growers with data-driven insights*

</div>