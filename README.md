# Toyota GR86

This repository contains signal set configurations for the Toyota GR86, organized by model year and version. The files are structured to allow for easy differentiation between model generations and other vehicle parameters, ensuring accurate signal mapping for each version of the Toyota GR86.

## About Toyota GR86 Generations

The Toyota GR86 has gone through two main generations, with the second being a significant redesign of the original 86:

- **First Generation (2012-2020)**: Initially launched as the Toyota GT86 (or simply Toyota 86 in some markets), this model was developed in collaboration with Subaru. It featured a naturally aspirated 2.0L boxer engine producing 200 hp, known for its lightweight design and rear-wheel drive configuration. The first generation received a facelift in 2017 with minor exterior updates and slight performance improvements.

- **Second Generation (2021-present)**: Rebranded as the GR86 under Toyota's Gazoo Racing lineup, the second generation brought significant improvements while maintaining the spirit of the original. Key changes include a larger 2.4L boxer engine producing 228 hp, improved chassis rigidity, and updated styling while keeping the fundamental front-engine, rear-wheel-drive layout. This generation features enhanced interior quality and modernized technology features. [[Toyota GR86 Official Page]](https://www.toyota.com/gr86/)

## Repository Structure

The directory is organized as follows:

```plaintext
signalsets/
  └── v3/
      ├── default.json        # Default configuration (applies to Second Generation and future models)
      └── 2012-2020.json      # Override configuration for First Generation (2012-2020)
```

- **default.json**: Acts as the primary configuration file, covering models from 2021 onwards (Second Generation). This file will serve as the default fallback for any years not specified by an override file.

- **2012-2020.json**: A specific configuration override for First Generation models (2012-2020), differentiating these years from the baseline configuration in `default.json`.

If a new generation is introduced in the future, a new JSON file (e.g., `2021-2027.json`) can be created to lock in the second-generation configuration, allowing `default.json` to reflect the latest specifications.

## Usage

Each JSON file in the `v3/` directory corresponds to a specific model year range. This structure enables compatibility with various vehicle parameters and generations. If new versions of the Toyota GR86 are released, they can be easily integrated by adding new JSON files, e.g., `2028+.json`.

## Related resources

- https://github.com/timurrrr/RaceChronoDiyBleDevice/blob/master/can_db/ft86_gen2.md
- https://docs.google.com/spreadsheets/d/1S_lZcHgQSWaoItuRQDe7_oxcpEvJl8Gh-JTX2d60Svc/edit?gid=0#gid=0

## Contributing

Contributions are welcome! If you would like to add support for additional model years or other configurations, please open an issue or submit a pull request.

1. Fork the repository
2. Create a new branch for your changes
3. Commit your changes and open a pull request with a detailed description

## Issues

If you encounter any issues or would like to discuss improvements, please feel free to open an issue. We encourage collaboration and appreciate feedback to make the repository as accurate and useful as possible.
