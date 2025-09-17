# Travel List

Travel List is a small React application for keeping track of what you need to pack for a trip. Add items with quantities, check them off as you go, and clear the list when you are ready to plan the next adventure.

## Features

- Manage a shared list of packing items that lives in the `App` component state.
- Add new entries with a quantity selector (`Form`) and automatically generated identifiers.
- Toggle items between packed and unpacked states straight from the list (`Item`).
- Sort by input order, description, or packed status to match the way you like to plan (`PackingList`).
- Keep an eye on progress with a live completion summary, including a celebratory message at 100 percent (`Stats`).
- Prevent accidental mass deletions with a clear-all confirmation prompt.

## Tech Stack

- React 19 with functional components and hooks (`useState`).
- Create React App tooling for development, bundling, and testing.
- Global styles defined in `src/index.css`.

## Getting Started

### Prerequisites

- Node.js 18 or newer is recommended (Create React App requires at least Node 14.0.0).
- npm 9 or newer (ships with recent Node installations).

### Installation

1. Install dependencies:
   ```bash
   npm install
   ```
2. Start the development server:
   ```bash
   npm start
   ```
   The app runs at http://localhost:3000 with hot reloading.

### Additional Scripts

- `npm test` - Launches Jest in watch mode.
- `npm run build` - Produces an optimized production build in `build/`.
- `npm run eject` - Copies the configuration files so you can customize the tooling (irreversible).

## Project Structure

```
src/
  components/
    App.js          # Root component containing packing list state
    Form.js         # Item creation form with quantity dropdown
    PackingList.js  # List rendering, sorting controls, and clear action
    Item.js         # Individual list entry with toggle and delete actions
    Stats.js        # Footer summary of packing progress
    Logo.js         # App title banner
  index.js          # CRA entry point
  index.css         # Global styles
```

## Contributing

Pull requests are welcome. Please open an issue first to discuss significant changes. Keep the packing experience simple and focused.

## License

This project is shared for learning purposes and does not currently specify a license. Add one if you plan to publish or redistribute.
