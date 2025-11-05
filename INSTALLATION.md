# Package Installation Guide

## Required Packages for Bayesian Cosmology Assignment

### Quick Installation (Recommended)

Open a terminal in the project directory and run:

```bash
pip install -r requirements.txt
```

### Individual Package Installation

If you prefer to install packages one by one:

```bash
pip install numpy
pip install matplotlib
pip install scipy
pip install jupyter
pip install notebook
```

### Using Conda (Alternative)

If you use Anaconda/Miniconda:

```bash
conda install numpy matplotlib scipy jupyter notebook
```

### Package Details

1. **NumPy** (≥1.21.0)
   - Purpose: Numerical computations, array operations
   - Used for: MCMC calculations, data storage, statistical operations

2. **Matplotlib** (≥3.4.0)
   - Purpose: Data visualization
   - Used for: All plots (trace plots, histograms, 2D posteriors, etc.)

3. **SciPy** (≥1.7.0)
   - Purpose: Scientific computing and statistics
   - Used for: Kernel density estimation (KDE), statistical functions

4. **Jupyter** (≥1.0.0)
   - Purpose: Interactive notebook interface
   - Used for: Running the notebook environment

5. **Notebook** (≥6.4.0)
   - Purpose: Jupyter notebook server
   - Used for: Serving the notebook application

### Verification

To verify packages are installed correctly, run in Python:

```python
import numpy as np
import matplotlib.pyplot as plt
import scipy
import jupyter

print("NumPy version:", np.__version__)
print("Matplotlib version:", plt.matplotlib.__version__)
print("SciPy version:", scipy.__version__)
print("Jupyter version:", jupyter.__version__)
print("\nAll packages installed successfully!")
```

### Troubleshooting

**If installation fails:**

1. Update pip first:
   ```bash
   pip install --upgrade pip
   ```

2. Try installing with user flag:
   ```bash
   pip install --user numpy matplotlib scipy jupyter notebook
   ```

3. For permission errors on Linux/Mac:
   ```bash
   sudo pip install numpy matplotlib scipy jupyter notebook
   ```

**If you get ImportError:**

Make sure you're using the correct Python environment where packages were installed. Check with:

```bash
which python
which pip
```

### After Installation

Launch the notebook:

```bash
jupyter notebook bayesian_cosmology_assignment.ipynb
```

Or simply:

```bash
jupyter notebook
```

Then open `bayesian_cosmology_assignment.ipynb` from the browser interface.

---

## Additional Notes

- All packages are standard scientific Python libraries
- No special configuration needed
- The notebook will run successfully once these 5 packages are installed
- No GPU or special hardware required
- Expected runtime: 2-3 minutes for complete analysis

---

**You're all set to run the assignment!**
