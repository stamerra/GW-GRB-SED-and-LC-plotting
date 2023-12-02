# GW-GRB-SED-and-LC-plotting
Analyzes and plots data from Gamma-Ray Burst (GRB) simulations. It reads information from a FITS file, extracts relevant data, and generates plots for Spectral Energy Distribution (SED), Flux, and Lightcurve. Additionally, it checks if the SED is above sensitivity and estimates rough significance.


## Python Code Documentation: GRB Analysis and Plotting

### Overview:
The provided Python script analyzes and plots data from Gamma-Ray Burst (GRB) simulations. It reads information from a FITS file, extracts relevant data, and generates plots for Spectral Energy Distribution (SED), Flux, and Lightcurve. Additionally, it checks if the SED is above sensitivity and estimates rough significance.

### Code Structure:

1. **Importing Libraries:**
   - Utilizes libraries such as `astropy` for FITS file handling, `numpy` for numerical operations, and `matplotlib` for plotting.

2. **Setting Parameters:**
   - Defines simulation file number (`NSimFile`), print preference (`Print`), directory paths, and file names.

3. **Reading FITS File:**
   - Opens and reads the FITS file containing GRB simulation data.
   - Extracts header information, energy, time, and spectrum data.

4. **Extracting Relevant Information:**
   - Retrieves important parameters like isotropic energy (`Eiso`), distance (`Distance`), and angle (`Angle`) from the FITS file.

5. **Filling Arrays with Spectra and Lightcurves:**
   - Populates arrays with spectral and lightcurve data at different time intervals.

6. **Plotting SED, Flux, and Lightcurve:**
   - Uses `matplotlib` to create plots for Spectral Energy Distribution (SED), Flux, and Lightcurve.
   - Overlaying reference curves and sensitivity data on the plots.

7. **Checking Sensitivity and Estimating Significance:**
   - Evaluates if the SED is above sensitivity levels.
   - Estimates rough significance based on flux differences at various time intervals.

### Usage:

- The script requires Python and relevant libraries installed.
- Modify parameters like `NSimFile`, `Print`, and file paths based on specific use cases.
- Execute the script to generate plots and analyze GRB simulation data.

### Output:

- The script produces plots of SED, Flux, and Lightcurve in the specified directory (`WorkDir`).
- If the `Print` option is set to 'Y', it saves the plots as PNG files.

### Notes:

- Ensure FITS files follow the expected format and contain necessary data fields.
- The script provides insights into the characteristics of GRB simulations, including their SED, Flux, and temporal evolution.

---
