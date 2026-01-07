# C2PA Privacy Inspector

**A Python tool to audit the "behavioral fingerprints" hidden inside AI Content Credentials.**

![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)
![Python](https://img.shields.io/badge/python-3.10+-blue.svg)
![Status](https://img.shields.io/badge/Status-Research_Prototype-orange.svg)

## The Problem
Moving into 2026, the **Coalition for Content Provenance and Authenticity (C2PA)** standard could soon become a default for AI transparency. While it fights misinformation, it also introduces a new privacy risk: **Metadata Persistence.**

Every "signed" image carries a history of:
* **Tools used** (e.g., specific Adobe Photoshop versions, OpenAI models).
* **Edit history** (provenance chains).
* **Ingredient data** (original assets merged into the final image).

This tool allows researchers and developers to **inspect** and **audit** what data their AI-generated media is leaking.

## Features
* **Manifest Extraction**: Pulls the raw JSON manifest from C2PA-signed images (JPEG, PNG, WebP).
* **Privacy Flagging**: Automatically flags high-risk metadata (e.g., location data, unique software IDs).
* **Ingredient Mapping**: Visualizes the chain of assets that created the final image.

## Installation

```bash
# Clone the repository
git clone [https://github.com/TechEnginHER/c2pa-privacy-inspector.git](https://github.com/TechEnginHER/c2pa-privacy-inspector.git)

# Install dependencies
pip install c2pa-python
```
## Usage
python inspector.py path/to/image.jpg

## Contributing
Contributions are welcome! If you find a C2PA-signed image that breaks the parser or exposes new metadata fields, please open an issue.

1. Fork the Project

2. Create your Feature Branch `(git checkout -b feature/AmazingFeature)`

3. Commit your Changes `(git commit -m 'Add some AmazingFeature')`

4. Push to the Branch `(git push origin feature/AmazingFeature)`

5. Open a Pull Request
