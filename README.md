# PSI5123 Problem Set

Solutions for the first problem set of PSI5123 Speech and Audio Machine Learning.

Developed in Python using NumPy, SciPy, Librosa, and Matplotlib.

---

## Author

MSc João Victor Colombari Carlet  
NUSP: 5274502

---

## Repository Structure

```text
.
├── input_figures
│   ├── f1.png
│   ├── ...
│   └── f6.png
├── lista_1.pdf
├── main.ipynb
├── notebooks_class
│   └── I will gitignore these files since they are not mine..
├── notes.pdf
├── README.md
├── SA1.WAV
├── SIFT_paper
│   └── I will gitignore this file since they are IEEE's..
└── venv
```

---

## Main Notebook

All exercises and solutions are available in:

```text
main.ipynb
```

Some of my notes for the set are available (just for reference) in:
```text
notes.pdf
```

The notebook contains:
- mathematical derivations,
- theoretical discussions,
- waveform and spectrogram visualizations,
- pitch estimation implementations,
- comparisons between algorithms,
- and probability/statistical analyses.

---

## Topics Covered

### 1. Spectrogram Interpretation
- Manual construction of signals from spectrogram descriptions
- STFT visualization using Librosa
- Linear and exponential sweeps
- Multi-tone synthesis

### 2. Spectrogram Analysis
- Sampling frequency estimation
- Frequency resolution
- Window size determination
- Hop size estimation

### 3. Speech Segmentation
- Voiced sounds
- Unvoiced sounds
- Silence regions
- Speech production discussion

### 4. Fundamental Frequency Estimation

#### Standard Autocorrelation
- Manual segmentation
- Manual autocorrelation implementation
- Peak picking
- F0 estimation constraints

#### SIFT Algorithm
- LPC inverse filtering
- Residual extraction
- Residual autocorrelation
- Comparison against standard autocorrelation

### 5. Autocorrelation Function Properties
Verification of:
- symmetry,
- peak at zero,
- positivity at the origin.

### 6. Probability Density Functions
- Expected value
- Variance
- Gaussian and uniform distributions

---

## Environment Setup

Create a virtual environment:

```bash
python3 -m venv venv
```

Activate the environment:

```bash
source venv/bin/activate
```

Install Jupyter Notebook and the required libraries:

```bash
pip install notebook numpy scipy matplotlib librosa
```

Launch Jupyter:

```bash
jupyter notebook
```

And for dependencies run the first block of 

```text
main.ipynb
```

---

## Running

Open the notebook with Jupyter:

```bash
jupyter notebook main.ipynb
```

or with VSCode/JupyterLab.

---

## References

- Rabiner, L. R., Schafer, R. W. — *Digital Processing of Speech Signals*
- Markel, J. D. — *The SIFT Algorithm for Fundamental Frequency Estimation*
- Librosa Documentation
- PSI5123 lecture material (pdf and video files)