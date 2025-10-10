# Amazon Video Game Reviews Analysis

## Overview
This project analyzes Amazon video game product reviews and metadata to gain insights into:
- Rating distributions and patterns
- Product categorization analysis
- Category-rating relationships
- Market segmentation trends

## Dataset
The analysis uses two JSONL files from the [Amazon Reviews Dataset 2023](https://amazon-reviews-2023.github.io/):
- `Video_Games.jsonl`: Contains customer reviews with ratings and feedback
- `meta_Video_Games.jsonl`: Contains product metadata including categories and details

### Data Structure
#### Reviews Data (`Video_Games.jsonl`)
- `asin`: Amazon Standard Identification Number
- `reviewerID`: Unique reviewer identifier
- `reviewText`: Full review content
- `summary`: Review summary/title
- `overall`: Rating (1-5 scale)
- `helpful`: [helpful votes, total votes]

#### Metadata (`meta_Video_Games.jsonl`)
- `parent_asin`: Product identifier
- `title`: Game title
- `categories`: Product categories/genres
- `details`: Product specifications
- `average_rating`: Mean rating
- `rating_number`: Number of ratings
- `store`: Platform information
- `price`: Product price

## Analysis Components
The project includes several key analyses:

1. **Rating Distribution Analysis**
   - Statistical summary of ratings
   - Distribution visualization
   - Outlier identification

2. **Product Categorization**
   - Category frequency analysis
   - Multi-category product analysis
   - Category-rating correlation

3. **Market Insights**
   - Popular category identification
   - Rating patterns across categories
   - Product diversity analysis

## Requirements
```
pandas>=1.5.0
matplotlib>=3.5.0
seaborn>=0.12.0
```

## Usage
The analysis is contained in Jupyter notebooks:
1. `notebooks/01 Data loading and validaiton.ipynb`
   - Data loading and validation
   - Basic exploratory analysis
   - Category analysis
   - Rating distribution analysis

## Installation
1. Clone the repository:
```bash
git clone https://github.com/YuriyKimV/amazon_product_review.git
```

2. Install required packages:
```bash
pip install -r requirements.txt
```

3. Place the dataset files in the `data/` directory:
   - `data/Video_Games.jsonl`
   - `data/meta_Video_Games.jsonl`

## License
This project is licensed under the MIT License - see the LICENSE file for details.

## Author
YuriyKimV
