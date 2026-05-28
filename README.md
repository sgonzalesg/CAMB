# CAMB & CMB Anisotropy Testing Repository

Welcome to my dedicated workspace for testing and running **CAMB** (Code for Anisotropies in the Microwave Background). This repository focuses on computational cosmology, specifically the generation of theoretical angular power spectra ($C_\ell$), matter power spectra $P(k)$, and the subsequent creation of full-sky maps.

## Repository Structure

* **`Power_Spectrum_Perturbations/01_camb_configurations`**: Core configuration files (`.ini`), parameter sweeps, and scripts to run CAMB across different cosmological models (standard $\Lambda$CDM and extensions).
* **`Power_Spectrum_Perturbations/02_power_spectra_analysis`**: Jupyter notebooks dedicated to extracting and plotting the output spectra, including Temperature (TT), Polarization (EE, BB), and Cross-spectra (TE).
* **`Power_Spectrum_Perturbations/03_healpy_simulations`**: Scripts strictly utilizing the **HEALPix** framework (via the `healpy` library) to generate, visualize, and manipulate full-sky spherical maps directly from CAMB's theoretical $C_\ell$ outputs. 
* **`Power_Spectrum_Perturbations/04_planck_data_comparison`**: Workflows designed to compare our theoretical CAMB runs against actual observational data from the Planck mission.
* **`Power_Spectrum_Perturbations/05_utility_scripts`**: Helper functions for unit conversions, formatting outputs, and managing data pipelines.

## Tech Stack

* **Main Language:** Python 3.x
* **Cosmology Codes:** CAMB, healpy (HEALPix)
* **Data Analysis & Visualization:** NumPy, SciPy, Matplotlib
* **Version Control:** Git & GitHub

## Installation and Usage

To run the CAMB python wrapper and map-making tools locally, set up your environment as follows:

1. Clone this repository:
```bash
   git clone [https://github.com/your-username/camb-cmb-testing.git](https://github.com/your-username/camb-cmb-testing.git)
   cd camb-cmb-testing
```

2. Create and activate a virtual environment:
```bash
   python -m venv venv
   source venv/bin/activate  # On Linux/Mac
   venv\Scripts\activate     # On Windows
```

3. Install CAMB, healpy, and other dependencies:
```bash
   pip install camb healpy numpy scipy matplotlib jupyter
```
