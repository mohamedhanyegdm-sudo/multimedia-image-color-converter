# Image Color Conversion GUI

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/mohamedhanyegdm-sudo/multimedia-image-color-converter/blob/main/Multimedia_Project_Section1.ipynb)

A small interactive GUI, built as a Jupyter / Google Colab notebook, for a Multimedia course project. Upload an image, then press a button to see it converted to another color model.

## Features

- **Upload** any image from your computer (PNG, JPG, ...).
- **RGB**: show the original image.
- **Grayscale**: RGB to grayscale conversion (Section 1, by Mohamed Hany).
- **Binary**: black and white image using a threshold, adjustable with a slider (0 to 255, default 128).
- **CMY**: RGB to CMY conversion.
- **CMYK**: RGB to CMYK conversion, shown as the four separate channels (C, M, Y, K).

The conversion functions (`to_gray`, `to_binary`, `to_cmy`, `to_cmyk`) are plain NumPy / OpenCV code, so you can reuse them outside the GUI.

## How to run in Google Colab

1. Click the **Open In Colab** badge above.
2. Choose **Runtime > Run all**.
3. In the last cell, press **Upload Image** and pick a file.
4. Press any of the buttons (RGB, Grayscale, Binary, CMY, CMYK). Move the slider to change the Binary threshold.

## How to run locally

```bash
pip install -r requirements.txt jupyter
jupyter notebook Multimedia_Project_Section1.ipynb
```

Then run all cells. The GUI uses `ipywidgets`, so it needs Jupyter Notebook or JupyterLab with widget support (or Colab).

## Project files

- `Multimedia_Project_Section1.ipynb`: the notebook (imports, conversion functions, GUI).
- `requirements.txt`: Python packages used.

## Team

Team project for the Multimedia course, Faculty of Computers and Information, Sinai University.

- Ahmed Yasser Ali
- Adham Reda Faisal
- Mohamed Hany
- Ali Mahmoud Mohamed
- Ahmed Ibrahim

## Notes

The notebook implements Section 1 (RGB to Grayscale) together with the Binary, CMY and CMYK conversions, all in the same GUI.
