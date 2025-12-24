![CarEyeSmall](https://github.com/user-attachments/assets/ae71ff4b-bbc3-4aa8-af82-57bc4482cde1)

## 📖 Table of Contents

1.  [Overview](#-overview)
2.  [Project Structure](#-project-structure)
3.  [Features](#-features)
4.  [Prerequisites](#-prerequisites)
5.  [Installation](#-installation)
6.  [Usage](#-usage)
7.  [Contributing](#-contributing)
8.  [License](#-license)
9.  [Acknowledgments](#-acknowledgments)

## 🚀 Overview

CarEye: A learning repo focusing on automotive camera systems—exploring hardware architectures, software pipelines, and key algorithms like demosaic, HDR, and CNN-based perception. Dive into sensor setups, ISP fundamentals, classic/ML-based algorithms, and hands-on implementations. 
Tags: automotive-camera, sensor setups, ISP fundamentals, classic/ML-based algorithms, and hands-on implementations.

## 📁 Project Structure
CarEye/<br>
├── docs/ # Datasheets, research papers, and learning notes<br>
├── hardware/ # Hardware schematics, sensor specifications<br>
├── firmware/ # Camera drivers and configuration scripts<br>
├── src/ # Core algorithm source code<br>
│ ├── isp/ # Image Signal Processing (e.g., Demosaic, HDR)<br>
│ ├── perception/ # Computer Vision (e.g., object detection, lane detection)<br>
│ ├── utils/ # Utility functions (image I/O, logging)<br>
│ ├── core/ # System core (data flow management)<br>
│ └── main.py # Main application entry point<br>
├── config/ # Configuration files (YAML)<br>
├── tests/ # Unit and integration tests<br>
├── data/ # Sample video/images and output data<br>
├── third_party/ # Third-party libraries and tools<br>
├── tools/ # Helper scripts for analysis and visualization<br>
├── README.md # This file<br>
└── requirements.txt # Python dependencies<br>


## ✨ Features

*   **Hardware Analysis:** Study of camera modules, lenses, and sensor interfaces.
*   **ISP Pipeline:** Implementation of fundamental algorithms like **Demosaic**, WDR, and noise reduction [1](@ref).
*   **Computer Vision:** Development and testing of perception algorithms for the automotive environment.
*   **Modular Design:** The codebase is organized to be easily extensible for new experiments.
*   **Documentation:** A growing collection of notes and references on automotive camera technology.

## ⚙️ Prerequisites

Ensure you have the following installed on your system:
*   **Python 3.8+**
*   **pip** (Python package manager)
*   **Git**
*   (Optional) A C++ compiler (e.g., g++) if native extensions are used.

## 📥 Installation

Follow these steps to set up the project locally:

1.  **Clone the repository:**
   git clone https://github.com/<your-username>/CarEye.git
bash
cd CarEye

2.  **(Recommended) Create a virtual environment:**
bash
python -m venv venv
source venv/bin/activate # On Windows: venv\Scripts\activate
3.  **Install Python dependencies:**
bash
pip install -r requirements.txt

## 🎮 Usage

After installation, you can explore different modules.
1.  **Basic Demo:**
Run the main script to see a basic pipeline in action (update the path to your data file):
bash
python src/main.py --input data/samples/sample_video.avi
2.  **ISP Module:**
To test the demosaic algorithm on a raw image:
python
from src.isp.demosaic import demosaic_vvg
processed_image = demosaic_vvg(raw_image_array)

## 🤝 Contributing

Contributions are highly welcome! Whether it's fixing a typo, adding a new algorithm, or improving documentation, your input is valuable. Please feel free to submit Pull Requests (PRs) or open issues for discussions [6,7](@ref).

1.  Fork the Project.
2.  Create your Feature Branch (`git checkout -b feature/AmazingFeature`).
3.  Commit your Changes (`git commit -m 'Add some AmazingFeature'`).
4.  Push to the Branch (`git push origin feature/AmazingFeature`).
5.  Open a Pull Request.

Please read `CONTRIBUTING.md` for detailed guidelines.

## 📄 License

This project is distributed under the MIT License. See the `LICENSE` file for more information [6](@ref).

## 🙏 Acknowledgments

*   This project is inspired by the need for open educational resources in automotive technology.
*   Thanks to the open-source community for providing invaluable tools and libraries.
*   References to various technical datasheets and research papers that guided the learning process.
