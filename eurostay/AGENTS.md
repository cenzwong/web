# Agent Instructions

This repository contains the source code for EuroStay, a guide for EU hotel brands.

## Common Tasks

### Adding a New Hotel Entry

To add a new hotel brand to the guide, follow these steps:

1.  **Create a Data File**:
    *   Create a new JSON file in the `data/` directory.
    *   The filename should be lowercase and kebab-case (e.g., `my-new-hotel.json`).
    *   The content must follow this JSON structure:
        ```json
        {
          "name": "Brand Name",
          "category": "category_key",
          "vibe": "Short description of the vibe",
          "desc": "Longer description of the hotel brand.",
          "price": "€€",
          "icon": "lucide-icon-name"
        }
        ```
    *   **Fields**:
        *   `name`: The display name of the hotel brand.
        *   `category`: One of `tech`, `classic`, or `social`.
        *   `vibe`: A short, catchy phrase describing the atmosphere.
        *   `desc`: A brief paragraph describing the brand's features.
        *   `price`: Price range indicator using Euro symbols (`€`, `€€`, `€€€`).
        *   `icon`: A valid [Lucide icon](https://lucide.dev/icons/) name (e.g., `hotel`, `wifi`, `coffee`).

2.  **Register the File**:
    *   Open `index.html`.
    *   Locate the `loadBrandData` function in the script section.
    *   Find the `jsonFiles` array inside the `if (isLocal)` block.
    *   Add the name of your new JSON file to this list.

    ```javascript
    if (isLocal) {
        // ...
        jsonFiles = [
            "a-and-o.json",
            // ... existing files ...
            "my-new-hotel.json" // Add your file here
        ];
    }
    ```

    *Note: This step is required for the new entry to appear in the local development environment.*
