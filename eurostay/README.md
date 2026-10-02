# EuroStay

**EuroStay** is a modern, interactive guide to Europe's most popular budget hotel brands. It helps travelers decode the difference between "high-tech capsules" and "classic roadside value" to find the perfect stay without the high price tag.

## Features

*   **Brand Guide**: Browse a curated list of budget hotel chains.
*   **Smart Filtering**: Filter brands by experience type:
    *   *High-Tech*: For the gadget-loving solo traveler.
    *   *Classic Value*: Reliable comfort for families and business.
    *   *Social/Fun*: Hostels and hotels with a community vibe.
*   **Comparison Table**: At-a-glance comparison of price ranges, vibes, and key amenities.
*   **Regional Tips**: Insider advice on which brands dominate specific European regions.

## Tech Stack

This project is built as a lightweight static site with no heavy build steps.

*   **HTML5 & Vanilla JavaScript**: Core logic and structure.
*   **Tailwind CSS** (via CDN): Styling and responsive design.
*   **Lucide Icons** (via CDN): Iconography.
*   **JSON**: Data storage for hotel brands.

## Getting Started

Since this is a static site, you can run it with any simple HTTP server.

### Prerequisites

*   Python 3 (or any other local server tool like `serve`, `http-server`, etc.)

### Running Locally

1.  Clone the repository:
    ```bash
    git clone https://github.com/cenzwong/eurostay.git
    cd eurostay
    ```

2.  Start a local server:
    ```bash
    python -m http.server 8000
    ```

3.  Open your browser and navigate to:
    `http://localhost:8000/`

## Project Structure

*   `index.html`: The main entry point containing the UI and logic.
*   `data/`: Directory containing individual JSON files for each hotel brand.
*   `AGENTS.md`: Instructions for AI agents and developers on how to modify the codebase.

## Contributing

### Adding a New Hotel Brand

EuroStay is designed to be easily extensible. To add a new hotel brand:

1.  Add a new JSON file in the `data/` directory.
2.  Register the new file in `index.html` (for local development).

For detailed instructions on the data schema and process, please refer to **[AGENTS.md](./AGENTS.md)**.

## License

This project is for informational purposes only.
