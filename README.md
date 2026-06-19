# Interactive KPI Cards

A Power BI custom visual that displays a set of four interactive KPI cards with hover-to-reveal detail panels.

## Features

- **4 Interactive KPI Cards**: Display up to 4 key performance indicators in a single visual
- **Hover-to-Reveal Details**: Detailed information appears when hovering over cards
- **Dynamic Values**: Supports dynamic values from your data model
- **Change Pills**: Display period-over-period changes with conditional coloring (positive/negative/neutral)
- **Customizable Styling**: 
  - Configurable side accent colors for each card
  - Customizable background colors
  - Dynamic title and value colors
  - Adjustable font sizes
- **Icon Support**: Choose from 11 built-in icons for each card
- **No DAX Required**: Fully configurable from the Power BI format panel

## Installation

1. Download the `.pbiviz` file from the releases
2. In Power BI Desktop, go to **File** → **Import a custom visual** → **Import from file**
3. Select the `.pbiviz` file and click **Open**
4. The visual will appear in your Visualizations pane

## Usage

### Data Fields

- **Values**: Add 1-4 measures (each becomes one card)
- **Icons (SVG)** (Optional): One SVG text measure per card, in the same order as Values
- **Prior Period** (Optional): One prior period measure per card for change calculation

### Configuration

Use the Format panel to configure:

1. **General Settings**
   - Global value color (fallback)
   - Prior period label

2. **Card Settings** (for each card)
   - Title and title formatting (font size, color, bold)
   - Icon selection (1-11)
   - Accent/side color
   - Card background color
   - Value format and styling
   - Change pill display
   - Detail description text

### Icon Options

1. Users
2. Bar Chart
3. Trend Up
4. Dollar
5. Target
6. Cart
7. Star
8. Lightning
9. Award
10. Activity
11. Check

## Project Structure

```
interactive-kpi-cards/
├── assets/
│   └── icon.png              # Visual icon for Power BI
├── resources/
│   └── *.pbiviz.json         # Visual configuration and code
├── package.json              # Project metadata
└── README.md                 # This file
```

## Technical Details

- **Version**: 1.0.0.0
- **API Version**: 5.3.0
- **Author**: Interactive KPI Cards
- **Support**: https://github.com/interactiveKPICards/support

## Development

This visual is built as a Power BI custom visual using the Power BI Visuals API.

### Building from Source

To modify and rebuild this visual:

1. Extract the `.pbiviz` file (it's a ZIP archive)
2. Modify the code in `resources/*.pbiviz.json`
3. Update the icon in `assets/icon.png` if needed
4. Repackage as a `.pbiviz` file

## License

This project is provided as-is for use with Power BI.

## Support

For issues, feature requests, or support, please visit: https://github.com/interactiveKPICards/support
