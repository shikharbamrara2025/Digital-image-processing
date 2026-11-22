# Digital Image Processing

A collection of Google Colab/Jupyter notebooks covering image filtering and lossless compression techniques.

## Notebooks

| Notebook | Contents |
|---|---|
| [filters.ipynb](filters.ipynb) | RGB-to-HSI processing, spatial and frequency-domain filters, edge detection (including Prewitt), and image restoration. Filters are applied to the Intensity (I) component while Hue and Saturation are preserved. |
| [huffman_coding.ipynb](huffman_coding.ipynb) | Huffman coding: frequency analysis, code construction, encoding and decoding. |
| [arithmetic_encoding.ipynb](arithmetic_encoding.ipynb) | Arithmetic coding: probability intervals, encoding and decoding. |

## Run in Google Colab

1. Open the notebook you want from this repository.
2. Select **Open in Colab** if available, or download the `.ipynb` file and upload it to [Google Colab](https://colab.research.google.com/).
3. Run the cells from top to bottom.
4. In `filters.ipynb`, upload an RGB image when prompted.

## Requirements

The filters notebook uses NumPy, OpenCV, SciPy, and Matplotlib. In Google Colab, these are generally available; if needed, run `!pip install numpy scipy matplotlib opencv-python`.

## Notes

The restoration section demonstrates restoration using a simulated degradation with a known blur and noise model. Notch filter locations may need adjustment for the frequency peaks in a particular image. Arithmetic coding is an educational Decimal-based implementation rather than a production file codec.
