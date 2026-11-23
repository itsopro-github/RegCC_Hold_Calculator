# Reg CC Funds Availability Calculator

A comprehensive web-based calculator for determining funds availability based on federal Regulation CC (12 CFR Part 229) requirements.

## Features

- **Multiple Deposit Types Support**
  - Cash deposits
  - Electronic payments
  - Government/Official checks
  - On-Us checks
  - Local/Other checks
  - Nonproprietary ATM checks
  - New account checks

- **Smart Business Day Calculations**
  - Automatic weekend and federal holiday detection
  - Federal holidays calendar for 2026-2028
  - Deposit time cutoff handling (2pm default)
  - Business day counting algorithm

- **Regulatory Compliance**
  - New account hold logic (accounts 30 days or less)
  - Exception hold support
  - Large deposit threshold handling ($5,525 default per Reg CC)
  - $200 next-day availability minimum
  - Proper hold period calculations

- **Aggregate Availability Schedule**
  - Multiple deposit items in a single transaction
  - Prioritized availability by deposit type
  - Clear breakdown of when funds become available
  - Visual timeline of fund availability

- **User-Friendly Interface**
  - Clean, modern Material Design-inspired UI
  - Responsive layout for mobile and desktop
  - Real-time calculations
  - Add/remove multiple deposit items
  - Warning notifications for extended holds

## Usage

Simply open `index.html` in a web browser. No build process or server required.

```bash
open index.html
```

Or serve it locally:

```bash
python3 -m http.server 8000
# Then navigate to http://localhost:8000
```

## Technical Details

- **Built with**: React 18 (via CDN)
- **Styling**: Pure CSS with Material Design principles
- **No dependencies**: Single HTML file, runs entirely in the browser
- **No build process**: Uses Babel standalone for JSX transformation

## Regulation CC Overview

Regulation CC implements the Expedited Funds Availability Act, which requires banks to make funds from deposited checks available according to specified schedules:

- **Next Business Day**: Cash, electronic payments, government checks, on-us checks
- **Second Business Day**: Local checks (up to $5,525)
- **Fifth Business Day**: Nonproprietary ATM deposits
- **Extended Holds**: New accounts (30 days or less) and exception holds

## Project Structure

```
RegCC_Hold_Calculator/
├── index.html          # Main application file
└── README.md           # This file
```

## Future Enhancements

- Export/print availability schedule
- Save/load scenarios
- Custom holiday calendar management
- Integration with banking systems
- Multi-language support
- PDF generation for customer notices

## License

TBD

## Author

Haroun
