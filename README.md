Image Deblurring using Dimensionality Reduction

A Google Colab notebook that uses **NAFNet** (Nonlinear Activation Free Network) to restore and deblur images using deep learning.

Overview

This project applies the NAFNet model to remove blur from images. It provides an end-to-end pipeline — from uploading a blurry image to downloading the restored result — all within a Google Colab environment.

Getting Started
Run in Google Colab

Click the badge below to open the notebook directly in Colab:

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/NonnyN/Image_Deblurring/blob/main/ImageDebluring.ipynb)

 How It Works

The notebook follows these steps:

1. **Clone NAFNet** — Downloads the NAFNet model repository from GitHub
2. **Set up the environment** — Installs all required dependencies from `requirements.txt`
3. **Download pretrained model weights** — Fetches the pre-trained deblurring model via `gdown`
4. **Upload your image** — Upload any blurry image directly in Colab
5. **Run inference** — Passes the image through the NAFNet model to produce a sharp output
6. **Visualize results** — Displays the blurry input alongside the deblurred output side by side
7. **Download results** — Saves and downloads the result as a `.zip` file

Dependencies

All dependencies are installed automatically in the notebook. Key packages include:

| Package | Purpose |
|---|---|
| `torch` | Deep learning framework |
| `opencv-python` | Image reading and processing |
| `scikit-image` | Image display and metrics |
| `Pillow` | Image I/O |
| `numpy` | Array operations |
| `gdown` | Downloading model weights from Google Drive |
| `lmdb` | Dataset handling |
| `tqdm` | Progress bars |

 Repository Structure

Image_Deblurring/
│
├── ImageDebluring.ipynb   # Main Colab notebook
└── README.md              # Project documentation

Model

This notebook uses **NAFNet**, a state-of-the-art image restoration model developed by MEGVII Research.

- 📄 Paper: [Simple Baselines for Image Restoration (ECCV 2022)](https://arxiv.org/abs/2204.04676)
- 💻 Original Repo: [megvii-research/NAFNet](https://github.com/megvii-research/NAFNet)

Example Results

| Input (Blurry) | Output (Deblurred) |
|---|---|
| *(your blurry image)* | *(restored sharp image)* |

Author

**NonnyN**  
GitHub: [@NonnyN](https://github.com/NonnyN)

License

This project builds on NAFNet, which is licensed under the MIT License. See the [NAFNet repository](https://github.com/megvii-research/NAFNet) for details.
