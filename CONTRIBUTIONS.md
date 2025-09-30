# xcss-vendor-template: Contributor Guide

This repository serves as the template for creating and maintaining vendor-prefix data sets that will be integrated into the main xcss-vendors project.

## 🤝 Contributions and Integration

To become a contributor and have your vendor data set integrated, please follow these steps:

1. **Clone the Template:** Clone this repository (xcss-vendor-template) to your own account and begin structuring your vendor data according to the guidelines below.

2. **Create an Issue:** Once your repository is ready, create a new issue in the main xcss-vendors repository with the following details:
    - **Platform:** Mention the platform the contribution is for (e.g., browser by default).
    - **Vendor Prefix:** Mention the specific vendor prefix (e.g., o, ms, moz, webkit).
    - **Request:** The issue must explicitly request that your new repository be added as a submodule.

3. **Verification:** The core maintainers will review your repository structure and content against the guidelines.

4. **Submodule Addition:** Upon successful verification, your repository will be added as a submodule to xcss-vendors.

## ⚙️ Repository Structure and Data Guidelines

Your repository must adhere to the following rules to ensure proper export and integration:

1. File Inclusion and Exclusion
    - **Ignored Items:** All hidden files and folders (those starting with a .) will be ignored during the export process.
    - **File Type:** Only files ending with the .json extension will be processed for export. All other file types will be ignored.

2. Prefix Grouping by Year
The data must be organized into folders representing the year the prefixes were introduced or updated.
    - **Year Folder Format:** Group all prefixes corresponding to a specific year within a folder named in YYYY format (e.g., 2024, 2025).
    - **Template:** Use the existing .year folder as a guide. When adding new data for a new year, clone or copy the structure of the .year folder and rename it to the appropriate four-digit year.

## Example Directory Structure:

The structure must categorize prefixes by their CSS domain within year folders:

```

/
├── 2024/
│   ├── atrules.json
│   ├── attributes.json
│   ├── classes.json
│   ├── elements.json
│   └── values.json
├── 2025/
│   ├── atrules.json
│   ├── attributes.json
│   ├── classes.json
│   ├── elements.json
│   └── values.json
└── .year/  <-- Use this as the structural template
    ├── atrules.json
    ├── attributes.json
    ├── classes.json
    ├── elements.json
    └── values.json

```

## ⚖️ Licensing

All contributions and the entire contents of this repository are governed by the attached license.

The license file (LICENSE or LICENSE.txt) located in the repository root MUST NOT be modified under any circumstances. Any attempt to alter the licensing terms will result in the rejection of the contribution.