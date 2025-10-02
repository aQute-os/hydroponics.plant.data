# Hydroponics Plant Data

A comprehensive collection of plant data for use in hydroponic tower systems. This repository contains detailed information about growing various plants hydroponically, including pH levels, EC (electrical conductivity), light requirements, and phase-specific growing parameters.

## Purpose

This repository serves as a centralized database for hydroponic growers to access standardized plant growing parameters. Each plant entry includes:

- Recommended seed brands
- Phase-specific growing parameters (seedling, growth, flowering)
- EC and pH requirements for each phase
- Light requirements (spectrum, intensity, duration)
- Seeding information and tips
- Detailed growing guides

## Repository Structure

```
.
├── README.md          # This file
├── TEMPLATE.md        # Template for creating new plant entries
├── plants/            # Directory containing all plant data files
│   ├── tomato.md
│   ├── lettuce.md
│   └── ...
```

## Plant Data Format

Each plant is stored as a Markdown file with YAML frontmatter containing structured data. The file includes:

### YAML Frontmatter Structure

```yaml
---
name: "Plant Name"
scientific_name: "Scientific Name"
seed_brands:
  - "Brand 1"
  - "Brand 2"

phases:
  seedling:
    duration_days: X
    ec: X.X
    ec_unit: "mS/cm"
    ph: X.X
    lights:
      band: "spectrum type"
      intensity_percent: XX
      hours_per_day: XX
    notes: "Phase-specific notes"
    
  growth:
    duration_days: X
    ec: X.X
    ec_unit: "mS/cm"
    ph: X.X
    lights:
      band: "spectrum type"
      intensity_percent: XX
      hours_per_day: XX
    notes: "Phase-specific notes"
    
  flowering:
    duration_days: X
    ec: X.X
    ec_unit: "mS/cm"
    ph: X.X
    lights:
      band: "spectrum type"
      intensity_percent: XX
      hours_per_day: XX
    notes: "Phase-specific notes"

seeding:
  method: "description"
  depth_cm: X.X
  spacing_cm: XX
  temperature_celsius: XX-XX
  germination_days: X-X
  tips: "Seeding tips"
---
```

### Markdown Content

After the YAML frontmatter, each file contains detailed growing information including:
- Plant overview
- Recommended varieties
- Growth characteristics
- Harvest information
- Common issues and solutions
- Tips for success

## Data Fields Explained

### Phases

- **seedling**: Initial growth phase from germination to first true leaves
- **growth**: Vegetative growth phase where plant develops foliage
- **flowering**: Reproductive phase for fruiting/flowering plants (not applicable to leafy greens)

### EC (Electrical Conductivity)

Measured in mS/cm (millisiemens per centimeter), indicates nutrient concentration in the solution.
- Lower values (0.6-1.2): Leafy greens, seedlings
- Medium values (1.5-2.0): Most vegetables in growth phase
- Higher values (2.0-3.0): Fruiting plants in flowering phase

### pH Levels

Most hydroponic plants prefer pH between 5.5-6.5. Specific ranges optimize nutrient availability for each plant.

### Light Requirements

- **band**: Light spectrum (e.g., "Full spectrum", "Blue-heavy", "Red enhancement")
- **intensity_percent**: Light intensity as percentage of maximum
- **hours_per_day**: Photoperiod duration

## Contributing New Plants

To add a new plant to the database:

1. Copy `TEMPLATE.md` to `plants/[plant-name].md`
2. Fill in all YAML fields with accurate data
3. Write comprehensive growing information in the markdown section
4. Submit a pull request

### Data Sources

When contributing, please ensure data comes from reliable sources:
- Scientific literature
- Reputable hydroponic growing guides
- Personal growing experience with documented results
- Agricultural extension services

## Using This Data

This data can be used to:
- Program automated hydroponic systems
- Create growing schedules
- Set up monitoring and control parameters
- Educate new hydroponic growers
- Compare growing requirements across plants

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Current Plants

- [Basil](plants/basil.md) - Popular herb with intense flavor, ideal for continuous harvest
- [Lettuce](plants/lettuce.md) - Fast-growing leafy green, ideal for beginners
- [Tomato](plants/tomato.md) - Popular fruiting vegetable for hydroponics

## Future Additions

Planned plants to add:
- More herbs (cilantro, parsley, mint, oregano, thyme)
- Peppers (bell, jalapeño, cayenne)
- Cucumbers
- Strawberries
- Kale and other brassicas
- Spinach
- Arugula
- Microgreens
- Swiss chard
- Bok choy

## Contributing

Contributions are welcome! Please feel free to submit pull requests with new plant data or improvements to existing entries.
