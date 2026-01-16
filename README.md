[README.md](https://github.com/user-attachments/files/24672884/README.md)
# Waste Heat Recovery ROI Calculator

A professional web-based calculator for analyzing the financial returns of waste heat recovery systems using absorption chiller technology for power generation efficiency improvements.

## Overview

This calculator helps power plant operators, energy managers, and investors evaluate the economic viability of implementing intake air cooling systems powered by waste heat recovery from gas turbine generators.

## Features

### 🎯 Three Analysis Modes

1. **Quick Analysis** - Simple 4-input interface for rapid ROI estimates
2. **Detailed Engineering** - Comprehensive technical and financial modeling
3. **Scenario Comparison** - Side-by-side evaluation of multiple configurations

### 🌐 Bilingual Interface

- Full Chinese (中文) and English support
- Toggle switch for instant language switching
- Default language: Chinese

### 📊 System Visualization

- Technical schematic-style diagram showing the closed-loop system
- Real-time component animations (rotating turbine, pulsing coils, flowing heat)
- Live parameter updates as inputs change
- Status indicators with LED-style lights

### 📱 Fully Responsive

- Desktop-optimized layout (>1024px)
- Tablet-friendly design (768-1024px)
- Mobile-responsive with vertical component stacking (<768px)
- Touch-friendly interface

### 💰 Comprehensive Financial Analysis

- Simple payback period
- Net Present Value (NPV)
- Internal Rate of Return (IRR)
- Annual savings calculations
- 20-year cash flow projections
- Energy price escalation modeling
- O&M cost analysis

### 🔧 Technical Capabilities

- Climate zone-based assumptions
- Generator type selection (gas turbine, reciprocating, combined cycle)
- Customizable temperature parameters
- Power gain calculations based on intake air temperature reduction
- Cooling capacity estimation
- Heat recovery efficiency modeling

## Technology Stack

- **Pure HTML/CSS/JavaScript** - No external dependencies
- **Responsive Design** - CSS Grid and Flexbox
- **SpaceX-inspired UI** - Minimalist black and white aesthetic
- **Technical Schematic Style** - Wireframe components with subtle animations

## Installation & Deployment

### Local Development

1. Clone the repository:
```bash
git clone https://github.com/yourusername/waste-heat-recovery-calculator.git
cd waste-heat-recovery-calculator
```

2. Open `index.html` in your browser:
```bash
open index.html  # macOS
start index.html # Windows
xdg-open index.html # Linux
```

### GitHub Pages Deployment

1. Push to GitHub:
```bash
git add .
git commit -m "Initial commit"
git push origin main
```

2. Enable GitHub Pages:
   - Go to repository Settings
   - Navigate to "Pages" section
   - Select "main" branch and "/ (root)" folder
   - Click Save

3. Your calculator will be available at:
   `https://yourusername.github.io/waste-heat-recovery-calculator/`

### Custom Domain (Optional)

1. Add a `CNAME` file with your domain:
```bash
echo "your-domain.com" > CNAME
git add CNAME
git commit -m "Add custom domain"
git push
```

2. Configure DNS records at your domain registrar

## Usage Guide

### Quick Start

1. **Select Mode**: Choose "Quick Analysis" for simple calculations
2. **Enter Parameters**:
   - Generator capacity (MW)
   - Climate zone
   - Operating hours per year
   - Electricity price ($/kWh)
3. **Calculate**: Click "Calculate ROI" button
4. **Review Results**: View payback period, annual savings, and system diagram

### Advanced Analysis

1. Switch to "Detailed Engineering" mode
2. Input comprehensive technical parameters:
   - Ambient and target temperatures
   - Exhaust temperature
   - Power gain rates
   - Capacity factors
3. Configure financial parameters:
   - Capital costs
   - O&M expenses
   - Discount rates
   - Incentives
4. Analyze 20-year cash flow projections and NPV

### Scenario Comparison

1. Select "Scenario Comparison" mode
2. Define up to 3 different scenarios
3. Compare payback periods, NPV, and IRR side-by-side
4. Make data-driven investment decisions

## System Requirements

- Modern web browser (Chrome, Firefox, Safari, Edge)
- JavaScript enabled
- Minimum screen width: 320px (mobile compatible)
- Recommended: 1920x1080 or higher for desktop

## Browser Compatibility

- Chrome/Edge 90+
- Firefox 88+
- Safari 14+
- Mobile browsers (iOS Safari, Chrome Mobile)

## Configuration

### Customizing Default Values

Edit the HTML file to modify default parameters:

```javascript
// Line ~1250: Simple mode defaults
document.getElementById('capacity').value = "10";
document.getElementById('operating-hours').value = "7000";
document.getElementById('electricity-price').value = "0.12";

// Line ~1380: Detailed mode defaults
document.getElementById('ambient-temp').value = "35";
document.getElementById('target-temp').value = "15";
```

### Modifying Climate Assumptions

Update climate parameters around line 1750:

```javascript
const climateParams = {
    'hot-humid': { tempReduction: 20, powerGainRate: 0.65 },
    'hot-dry': { tempReduction: 22, powerGainRate: 0.70 },
    // Add custom climate zones here
};
```

## Contributing

Contributions are welcome! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## License

This project is licensed under the MIT License - see the LICENSE file for details.

## Support

For issues, questions, or feature requests:
- Open an issue on GitHub
- Contact: [your-email@example.com]

## Acknowledgments

- Designed for BROAD Air Conditioning
- Inspired by SpaceX's minimalist design philosophy
- Technical specifications based on industry-standard absorption chiller performance data

## Roadmap

- [ ] PDF report generation
- [ ] Export to Excel functionality
- [ ] Multi-currency support
- [ ] Integration with CRM systems
- [ ] API for programmatic access
- [ ] Advanced sensitivity analysis
- [ ] Regional cost databases
- [ ] Carbon offset calculations

## Version History

### v1.0.0 (2026-01-16)
- Initial release
- Three calculation modes
- Bilingual support (Chinese/English)
- Mobile-responsive design
- Technical schematic visualization
- Comprehensive financial modeling

---

**BROAD Air Conditioning** | Waste Heat Recovery Solutions
