# Playing Card Suit Classification (ANN)

This project trains and tests a simple Artificial Neural Network (ANN) to classify playing card images by suit using grayscale image features.

## Project Structure

- `Phase2/preprocess.py` – image preprocessing and dataset loading
- `Phase2/ann.py` – ANN model implementation
- `Phase2/train.py` – training script and weight export
- `Phase2/test.py` – single-image inference script
- `dataSet/` – training and test image data by class folders

## Requirements

- Python 3.10+
- `numpy`
- `opencv-python`
- `scikit-learn`

Install dependencies:

```bash
pip install numpy opencv-python scikit-learn
```

## Train

From the repository root:

```bash
cd Phase2
python train.py
```

This generates:

- `weights_input_hidden1.npy`
- `weights_hidden1_hidden2.npy`
- `weights_hidden2_output.npy`

## Test / Predict

From the repository root:

```bash
cd Phase2
python test.py
```

## Important Notes

- `train.py` and `test.py` currently use absolute Windows-style dataset paths.  
  Update those paths to match your local environment before running.
- Class mapping in the current setup:
  - `0 = Hearts`
  - `1 = Diamonds`
  - `2 = Clubs`
  - `3 = Spades`
