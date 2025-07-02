# Interactive Content Tool (ICT) v1.0

### ***A Custom Tool for Creating Interactive Schematics***
**ICT** is a standalone web application developed to streamline the process of creating interactive, responsive image maps. It was designed to solve the challenges of using standard online tools by offering a flexible and efficient workflow, specifically for integrating complex diagrams into knowledge-sharing platforms like Google Sites.

This tool is composed of two main modules: a **Google Drive Link Converter** and a powerful **Interactive Image Mapper**.

## Key Features :
- **Google Drive Integration**: Automatically converts standard Google Drive sharing links into direct, embeddable image URLs.

- **Interactive Canvas**: Load any image via URL and draw, move, and resize interactive rectangular zones with pixel-level control.

- **Snap-to-Grid**: An optional grid-snapping feature to perfectly align multiple zones for a clean and professional layout.

- **Zone Property Editor**: Easily assign a title (for tooltips), a hyperlink, a target destination (*_blank, _top*...), and a display color to each zone.

- **Configuration Management**: Save multiple mapping configurations by name directly in your browser's local storage. Load and delete saved configurations to manage different projects efficiently.

- **Automatic Code Generation**: Instantly generates the complete, clean, and responsive HTML *<map>* and JavaScript code required for seamless integration into any web page or G-Site embed module.

## Usage Guide
## Module 1: Google Drive Link Converter
This utility solves a common issue when trying to embed images hosted on Google Drive.

1. **Get Share Link**: In your Google Drive, right-click your image and get the shareable link. Ensure permissions are set to "Anyone with the link".

2. **Paste & Convert**: Paste the link (e.g., https://drive.google.com/file/d/FILE_ID/view?usp=sharing) into the converter's input field.

3. **Click Convert**: The tool will generate two outputs:

- A **direct image URL** (e.g., *https://googleusercontent.com/...*). This is the URL you will use in the Image Mapper below.

- A basic **HTML embed code** (*<img>* tag).

## Module 2: Interactive Image Mapper
This is the core of the ICT.

### Step 1: Loading an Image
Paste the **direct image URL** (obtained from the converter or any other source) into the "Image URL to map" input field.

Click *Load Image*. The image will appear on the canvas below, ready for mapping.

### Step 2: Creating and Editing Zones
- **To Create a Zone**: Click and drag your mouse over the desired area on the image. A rectangle will appear.

- **To Select a Zone**: Simply click inside an existing rectangle. It will be highlighted, and the "Edit selected zone" panel will appear.

- **To Edit Zone Properties:**

  - **Title (tooltip)**: The text that will appear on hover.

  - **Link URL**: The destination URL for the click. Leave blank for no link.

  - **Target**: How the link opens (e.g., *_blank* for a new tab).

  - **Color**: The color of the rectangle's border within the tool (for organizational purposes).

  - **To Move/Resize a Zone**: Click on a zone to select it. Drag from the center to move it, or drag one of the handles on its edges and corners to resize it.

### Step 3: Managing Configurations (Save & Load)
This feature is crucial for complex diagrams and allows you to save your work.

#### To Save:

- Click the *Save* button.

- Enter a descriptive name for your configuration (e.g., *h225_reg_cockpit_schema*).

- Your configuration is saved in your browser's local storage and will appear in the "*Saved Configurations*" list.

#### To Load:

- Click the *Load* button and type the name of the configuration you want to retrieve.

- Alternatively, simply click on the name of the desired configuration in the list displayed at the bottom of the page.

#### To Delete: 
Click the three-dot menu next to a configuration in the list and select "*Delete*".

### Step 4: Generating and Using the Final Code
Once your mapping is complete, all the necessary code is automatically generated in the "**Generated HTML Code**" text area.

Click the *Copy* button.

Paste this entire code block into an **"Embed"** -> **"Embed code"** module on your Google Site, or into any HTML page. 
The included JavaScript will automatically handle the responsiveness and interactivity.


-------------------------------------------------------

*This tool was developed by Paul GAUTIER during an internship at Airbus Helicopters (2025).*
