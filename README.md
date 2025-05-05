# 🏛️ Cultural Heritage Image Restoration Toolkit

## 📌 Problem Statement

Preserving cultural heritage often involves digitizing and restoring old, degraded, and artifact-laden documents, manuscripts, and photographs. Many such images suffer from yellowing, stains, low contrast, bleed-through, and various types of noise, making them hard to study, interpret, or archive digitally. Manual restoration is time-consuming and may lead to inconsistencies. Hence, an automated, reproducible solution is needed to restore these documents with high quality and measurable enhancement.

## 📝 Project Description

This project presents an **automated image processing pipeline** built using Python and OpenCV for enhancing and restoring degraded images of historical or culturally significant documents. The system corrects color imbalance, denoises, enhances contrast, removes stains/bleed-through, and sharpens details. It also provides objective evaluation metrics to assess the quality of enhancement such as **BRISQUE score**, **Shannon entropy**, and **RMS contrast**.

## 🚀 Features

- ✅ **Automatic color cast (de-yellowing) correction**
- 🧽 **Noise reduction** using both median and Non-local Means filters
- ⚙️ **Adaptive thresholding and morphological operations** to create accurate masks
- 🎨 **Inpainting** to remove bleed-through, cracks, and stains
- 📈 **CLAHE-based contrast enhancement** for improved readability
- 🔍 **Detail sharpening** using both convolution and unsharp masking
- 📊 **Quality evaluation metrics**: BRISQUE, entropy, and contrast
- 🖼️ **Intermediate and final image outputs** for transparency
- 📂 **Batch processing support** for folders of images

## 💡 Use Cases

- Digital restoration of **ancient manuscripts**, **rare books**, and **archival records**
- Preprocessing for **OCR (Optical Character Recognition)**
- Enhancing images for **museum digitization projects**
- Assisting researchers in **paleography**, **history**, and **archaeology**
- Creating cleaner inputs for **AI models** trained on historical texts

## ✅ Advantages

- **Fully automated**: Can process hundreds of images without manual intervention
- **Modular and customizable**: Easily tweak filter sizes, CLAHE limits, etc.
- **Objective metrics** for benchmarking image quality improvements
- **Open-source & reproducible**: No proprietary tools required
- **Scalable for institutions**: Universities, libraries, and museums can integrate into workflows

## 🧑‍🤝‍🧑 Team Members

- **Sanmitha S Shetty** – Image Processing Lead & Developer  
-**Shivani**- Research & Documentation
-**Thanvi**- Testing & Evaluation

## 📂 Folder Structure

```
Cultural-Heritage-Image-Restoration/
├── main.py                 # Main processing script
├── brisque_model_live.yml # BRISQUE model file
├── brisque_range_live.yml # BRISQUE range file
├── output_folder/         # All processed images and metrics saved here
├── README.md              # Project documentation
```

## ⚙️ Dependencies

- Python 3.x
- OpenCV (`opencv-python` and `opencv-contrib-python`)
- NumPy
- Matplotlib
- scikit-image (`skimage`)

Install using:

```bash
pip install opencv-python opencv-contrib-python numpy matplotlib scikit-image
```

## 📥 How to Run

1. Place your `.jpg` images inside the `image_folder` directory.
2. Ensure BRISQUE model files are in the same directory as the script.
3. Run the script:
```bash
python main.py
```
4. All enhanced images and metrics will be saved in `output_folder`.
