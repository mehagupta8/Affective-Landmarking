# Affective Landmarking Visualization

A web-based interactive visualization tool for analyzing and displaying emotional annotations created using Doccano. This project processes Doccano-annotated text data to create beautiful, interactive visualizations that show the emotional journey through text, highlighting different emotions and their progression across multiple annotators.

## Overview

This project takes JSONL files exported from Doccano, where text has been annotated with emotional labels, and creates interactive visualizations showing:
- Emotional progression through the text
- Comparison of emotional annotations across multiple subjects
- Statistical analysis of emotional patterns
- Interactive exploration of annotated segments

## Features

- Interactive emotion spectrum charts for each annotator
- Side-by-side comparison of emotional annotations
- Detailed emotional analysis and insights
- Support for multiple annotators/subjects
- Beautiful and modern UI with smooth animations
- Export of visualization data for further analysis

## Project Structure

```
doccano_affective_landmarking/
├── main.py              # Script for processing Doccano JSONL exports
├── index.html           # Main dashboard with all visualizations
├── *.emotion_chart.html # Individual emotion charts for each annotator
└── README.md            # Project documentation
```

## Data Format

The project expects JSONL files exported from Doccano with the following structure:
```json
{
  "text": "Sample text to be annotated",
  "labels": [
    [start_position, end_position, "emotion_label"],
    ...
  ]
}
```

## Installation

1. Clone the repository:
```bash
git clone https://github.com/yourusername/doccano_affective_landmarking.git
cd doccano_affective_landmarking
```

2. Install required dependencies:
```bash
pip install -r requirements.txt
```

## Usage

1. Export your annotated data from Doccano in JSONL format
2. Place the JSONL files in your project directory
3. Run the main script to process the data and generate visualizations:
```bash
python main.py
```

4. Open `index.html` in your web browser to view the interactive dashboard

## Visualization Features

- **Interactive Charts**: Hover over data points to see the annotated text and emotional labels
- **Emotional Analysis**: View statistical breakdowns of emotional annotations
- **Responsive Design**: Works on desktop and mobile devices
- **Full-Screen Mode**: Click on any chart to view it in full-screen mode
- **Detailed Insights**: Each visualization includes analysis of annotation patterns
- **Annotator Comparison**: Compare emotional annotations across different subjects

## Technical Details

- Built with Python for processing Doccano JSONL exports
- Uses Plotly.js for interactive visualizations
- Modern HTML5/CSS3 for responsive design
- JavaScript for interactive features

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Acknowledgments

- [Doccano](https://github.com/doccano/doccano) for the annotation framework
- Plotly.js for the visualization library

Citable using [![DOI](https://zenodo.org/badge/975172605.svg)](https://doi.org/10.5281/zenodo.15467834)
