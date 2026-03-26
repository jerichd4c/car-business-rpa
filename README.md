<a id="readme-top"></a>

<!-- PROJECT LOGO -->
<br />
<div align="center">
<h3 align="center">WhatsApp Sales Analysis RPA 📊</h3>

  <p align="center">
    Automates sales data analysis, visual reporting, and WhatsApp notification delivery via Twilio.
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul><a id="readme-top"></a>

<h3 align="center">WhatsApp Sales Analysis RPA 📊</h3>

  <p align="center">
    Automates sales data analysis, visual reporting, and WhatsApp notification delivery via Twilio.
  </p>
</div>

<!-- TABLE OF CONTENTS -->
<details>
  <summary>Table of Contents</summary>
  <ol>
    <li>
      <a href="#about-the-project">About The Project</a>
      <ul>
        <li><a href="#built-with">Built With</a></li>
      </ul>
    </li>
    <li>
      <a href="#getting-started">Getting Started</a>
      <ul>
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#project-structure">Project Structure</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

This application loads sales data, performs a consolidated analysis, generates metric charts, and sends a report via WhatsApp through Twilio.

Key Features:
* Data loading and validation from Excel (`data/Ventas_Fundamentos.xlsx`)
* Key metrics and top performing models, locations, and channels
* Automated graph generation in `outputs/graphs/`
* WhatsApp report delivery with Twilio
* Optional image hosting via imgbb
* Automatic fallback to simulation if Twilio limits are reached

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* [![Python][Python-badge]][Python-url]
* [![Pandas][Pandas-badge]][Pandas-url]
* [![Matplotlib][Matplotlib-badge]][Matplotlib-url]
* [![Twilio][Twilio-badge]][Twilio-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running, follow these steps.

### Prerequisites

* Python 3.10 or superior
* Windows recommended (PowerShell tested)
* Twilio account with WhatsApp enabled (for real delivery)
* imgbb account (optional) for image hosting

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/jerichd4c/car-business-RPA.git
   ```
2. Create and activate virtual environment
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```
3. Install dependencies
   ```sh
   pip install -r requirements.txt
   ```
4. Configure environment variables
   Copy `whatsapp_config.env.sample` to `whatsapp_config.env` and fill in your credentials.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

1. Create or verify sample data:
   ```powershell
   python create_sample_data.py
   ```

2. Execute the RPA process:
   ```powershell
   python main.py
   ```

The flow performs data validation, analysis, visualization, and sending (or simulation).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- PROJECT STRUCTURE -->
## Project Structure

```
main.py                         # Flow orchestration
create_sample_data.py           # Sample Excel generator
utils/
  data_loader.py                # Data loading/validation
  analyzer.py                   # Metrics calculations
  visualizer.py                 # Graph generation
  whatsapp_sender.py            # WhatsApp delivery & simulation
  image_uploader.py             # imgbb integration
outputs/
  graphs/                       # Generated PNG/JPG visualizations
  simulation_log.txt            # Simulation history
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Twilio](https://www.twilio.com/) for WhatsApp delivery
* [pandas](https://pandas.pydata.org/) and [matplotlib](https://matplotlib.org/) for analysis and visualization
* [imgbb](https://api.imgbb.com/) for image hosting

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/jerichd4c/car-business-RPA.svg?style=for-the-badge
[contributors-url]: https://github.com/jerichd4c/car-business-RPA/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/jerichd4c/car-business-RPA.svg?style=for-the-badge
[forks-url]: https://github.com/jerichd4c/car-business-RPA/network/members
[stars-shield]: https://img.shields.io/github/stars/jerichd4c/car-business-RPA.svg?style=for-the-badge
[stars-url]: https://github.com/jerichd4c/car-business-RPA/stargazers
[issues-shield]: https://img.shields.io/github/issues/jerichd4c/car-business-RPA.svg?style=for-the-badge
[issues-url]: https://github.com/jerichd4c/car-business-RPA/issues
[license-shield]: https://img.shields.io/github/license/jerichd4c/car-business-RPA.svg?style=for-the-badge
[license-url]: https://github.com/jerichd4c/car-business-RPA/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/jerichd4c

[Python-badge]: https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54
[Python-url]: https://www.python.org/
[Pandas-badge]: https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white
[Pandas-url]: https://pandas.pydata.org/
[Matplotlib-badge]: https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black
[Matplotlib-url]: https://matplotlib.org/
[Twilio-badge]: https://img.shields.io/badge/Twilio-F22F46?style=for-the-badge&logo=Twilio&logoColor=white
[Twilio-url]: https://www.twilio.com/
        <li><a href="#prerequisites">Prerequisites</a></li>
        <li><a href="#installation">Installation</a></li>
      </ul>
    </li>
    <li><a href="#usage">Usage</a></li>
    <li><a href="#project-structure">Project Structure</a></li>
    <li><a href="#acknowledgments">Acknowledgments</a></li>
  </ol>
</details>

<!-- ABOUT THE PROJECT -->
## About The Project

This application loads sales data, performs a consolidated analysis, generates metric charts, and sends a report via WhatsApp through Twilio.

Key Features:
* Data loading and validation from Excel (`data/Ventas_Fundamentos.xlsx`)
* Key metrics and top performing models, locations, and channels
* Automated graph generation in `outputs/graphs/`
* WhatsApp report delivery with Twilio
* Optional image hosting via imgbb
* Automatic fallback to simulation if Twilio limits are reached

<p align="right">(<a href="#readme-top">back to top</a>)</p>

### Built With

* [![Python][Python-badge]][Python-url]
* [![Pandas][Pandas-badge]][Pandas-url]
* [![Matplotlib][Matplotlib-badge]][Matplotlib-url]
* [![Twilio][Twilio-badge]][Twilio-url]

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- GETTING STARTED -->
## Getting Started

To get a local copy up and running, follow these steps.

### Prerequisites

* Python 3.10 or superior
* Windows recommended (PowerShell tested)
* Twilio account with WhatsApp enabled (for real delivery)
* imgbb account (optional) for image hosting

### Installation

1. Clone the repo
   ```sh
   git clone https://github.com/jerichd4c/car-business-RPA.git
   ```
2. Create and activate virtual environment
   ```powershell
   python -m venv .venv
   .\.venv\Scripts\Activate.ps1
   ```
3. Install dependencies
   ```sh
   pip install -r requirements.txt
   ```
4. Configure environment variables
   Copy `whatsapp_config.env.sample` to `whatsapp_config.env` and fill in your credentials.

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- USAGE EXAMPLES -->
## Usage

1. Create or verify sample data:
   ```powershell
   python create_sample_data.py
   ```

2. Execute the RPA process:
   ```powershell
   python main.py
   ```

The flow performs data validation, analysis, visualization, and sending (or simulation).

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- PROJECT STRUCTURE -->
## Project Structure

```
main.py                         # Flow orchestration
create_sample_data.py           # Sample Excel generator
utils/
  data_loader.py                # Data loading/validation
  analyzer.py                   # Metrics calculations
  visualizer.py                 # Graph generation
  whatsapp_sender.py            # WhatsApp delivery & simulation
  image_uploader.py             # imgbb integration
outputs/
  graphs/                       # Generated PNG/JPG visualizations
  simulation_log.txt            # Simulation history
```

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- ACKNOWLEDGMENTS -->
## Acknowledgments

* [Twilio](https://www.twilio.com/) for WhatsApp delivery
* [pandas](https://pandas.pydata.org/) and [matplotlib](https://matplotlib.org/) for analysis and visualization
* [imgbb](https://api.imgbb.com/) for image hosting

<p align="right">(<a href="#readme-top">back to top</a>)</p>

<!-- MARKDOWN LINKS & IMAGES -->
[contributors-shield]: https://img.shields.io/github/contributors/jerichd4c/car-business-RPA.svg?style=for-the-badge
[contributors-url]: https://github.com/jerichd4c/car-business-RPA/graphs/contributors
[forks-shield]: https://img.shields.io/github/forks/jerichd4c/car-business-RPA.svg?style=for-the-badge
[forks-url]: https://github.com/jerichd4c/car-business-RPA/network/members
[stars-shield]: https://img.shields.io/github/stars/jerichd4c/car-business-RPA.svg?style=for-the-badge
[stars-url]: https://github.com/jerichd4c/car-business-RPA/stargazers
[issues-shield]: https://img.shields.io/github/issues/jerichd4c/car-business-RPA.svg?style=for-the-badge
[issues-url]: https://github.com/jerichd4c/car-business-RPA/issues
[license-shield]: https://img.shields.io/github/license/jerichd4c/car-business-RPA.svg?style=for-the-badge
[license-url]: https://github.com/jerichd4c/car-business-RPA/blob/master/LICENSE.txt
[linkedin-shield]: https://img.shields.io/badge/-LinkedIn-black.svg?style=for-the-badge&logo=linkedin&colorB=555
[linkedin-url]: https://linkedin.com/in/jerichd4c

[Python-badge]: https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54
[Python-url]: https://www.python.org/
[Pandas-badge]: https://img.shields.io/badge/pandas-%23150458.svg?style=for-the-badge&logo=pandas&logoColor=white
[Pandas-url]: https://pandas.pydata.org/
[Matplotlib-badge]: https://img.shields.io/badge/Matplotlib-%23ffffff.svg?style=for-the-badge&logo=Matplotlib&logoColor=black
[Matplotlib-url]: https://matplotlib.org/
[Twilio-badge]: https://img.shields.io/badge/Twilio-F22F46?style=for-the-badge&logo=Twilio&logoColor=white
[Twilio-url]: https://www.twilio.com/
