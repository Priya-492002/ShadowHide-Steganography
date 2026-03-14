# ShadowHide-Steganography
​A Python-based steganography application that uses Least Significant Bit (LSB) encoding to hide and extract encrypted text within lossless images.
# ShadowHide - Secure Image Steganography
# ShadowHide - Secure Image Steganography

**ShadowHide** is a cybersecurity tool developed in Python that enables the concealment of secret text messages within digital images. By utilizing the **Least Significant Bit (LSB)** technique, this tool hides data in plain sight without altering the visual appearance of the carrier image.

## 🚀 Key Features
* **LSB Encoding:** Efficiently modifies the last bit of pixel RGB values to store binary data invisibly.
* **Data Integrity:** Implements a custom delimiter (`#####`) to ensure exact message extraction.
* **Lossless Support:** Specifically optimized for **PNG** format to prevent data corruption common in lossy formats like JPEG.
* **Modern Interface:** User-friendly GUI built with **CustomTkinter** for a professional dark-mode experience.

## 🛠️ Technical Insight
During development, I analyzed the impact of image compression on data hiding. I discovered that **JPEG's lossy compression** alters pixel values, which destroys hidden bits—this is why the initial tests with `.jpeg` files returned "No secret message found". Consequently, ShadowHide enforces the use of **PNG (Lossless)** format to guarantee 100% data recovery.

## 💻 Tech Stack
* **Language:** Python 3.12+
* **UI Framework:** CustomTkinter
* **Imaging Library:** Pillow (PIL)
* **Concepts:** Bitwise Operations, Steganography, Data Integrity

## 📂 Installation
1. Clone the repo: `git clone https://github.com/Priya-492002/ShadowHide-Steganography.git`
2. Install dependencies: `pip install customtkinter Pillow`
3. Run the app: `python shadow_hide2.py`
   
