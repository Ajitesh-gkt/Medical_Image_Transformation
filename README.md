# Medical Image Transformation: CT to MRI Conversion

This project implements a **Generative Adversarial Network (GAN)** pipeline to transform CT scans into MRI scans and includes an **image fetcher** script for preprocessing datasets. The goal is to aid medical imaging research by automating CT-to-MRI conversion and organizing datasets for further analysis.

## Features

1. **GAN Pipeline**:
   - Converts CT scans into MRI scans using a custom GAN architecture.
   - Trained on paired datasets of CT and MRI images.
   - Outputs high-quality MRI-like images from CT inputs.

2. **Image Fetcher**:
   - Splits a composite image containing CT, MRI, and Mask data into three individual folders:
     - **CT scans**
     - **MRI scans**
     - **Mask images**

## Project Files

- **`CycleGAN_CT_MRI_CT.ipynb`**: Jupyter notebook implementing the GAN model for CT-to-MRI conversion.
- **`fetcher.py`**: Python script to split composite images into separate directories for CT, MRI, and Mask images.

## Requirements

### Python Libraries

- Python 3.9+
- TensorFlow 
- OpenCV
- NumPy
- Matplotlib




## Setup and Usage

### 1. Image Fetcher
To split composite images into separate folders:
1. Place your composite images in the `data/composite/` directory.
2. Run the script:
   ```bash
   python image_fetcher.py
   ```
3. The CT, MRI, and Mask images will be saved in their respective directories under `data/`.

### 2. GAN Pipeline
1. Open the `CycleGAN_CT_MRI_CT.ipynb` notebook.
2. Follow the steps to preprocess data, train the GAN, and generate MRI-like images.



## Future Enhancements

- Expand the dataset with more paired CT-MRI examples.
- Optimize GAN architecture for better MRI resolution.
- Add support for additional modalities like PET scans.
