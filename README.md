# 3D Reconstruction from 2D Images

Project focused on building a tool that converts 2D images into 3D models using computer vision and machine learning techniques.

---

## 1. Project Overview

The goal of this project is to reconstruct 3D models from 2D images. The tool applies computer vision and machine learning techniques to infer depth and three-dimensional structure of objects from one or more images.

### Challenges

- A single image does not carry complete information about depth and geometry.
- 3D reconstruction requires advanced techniques to infer the three-dimensional structure from limited data.

---

## 2. Technologies

| Technology | Purpose |
|---|---|
| **Python** | Main development language |
| **OpenCV** | Image processing and feature detection |
| **PyTorch** | Neural network implementation and training |
| **MiDaS** | Pre-trained model for depth estimation |
| **Trimesh** | 3D mesh generation and manipulation |
| **Open3D** | 3D data visualization and processing |
| **Blender** | 3D model visualization and editing |

---

## 3. Input Image Guidelines

To get the best results, the input image matters as much as the model. Follow these recommendations:

**Recommended:**

- ✅ A single object per image
- ✅ Standard front view of the object
- ✅ White, monochrome or removed background

**Not recommended:**

- ⚠️ Text on the image
- ⚠️ Multiple objects in one image
- ⚠️ Complex or cluttered background
- ❌ Inappropriate imagery, including harmful, offensive or NSFW content

---

## 4. Results

### 4.1 Basic 3D Models

**Cube:**
![Cube](resultados/cubo.png)

**Sphere:**
![Sphere](resultados/esfera.png)

### 4.2 Depth Estimation

**Depth Map:**
![Depth Map](resultados/mapa_profundidade.png)

### 4.3 Generated 3D Meshes

**3D mesh from a 2D image:**
![3D Mesh](resultados/malha_3d.png)

### 4.4 Complex Models

**Reconstruction of complex objects:**
![Complex Object](resultados/objeto_complexo.png)

---

## 5. How to Run

1. Clone the repository:

```sh
git clone https://github.com/guavovic/3d-reconstruction-from-2d-images.git
cd 3d-reconstruction-from-2d-images
```

2. Create and activate a virtual environment:

```sh
virtualenv venv
source venv/bin/activate   # Linux/Mac
venv\Scripts\activate      # Windows
```

3. Install the dependencies:

```sh
pip install -r requirements.txt
```

4. Run the scripts:

```sh
python scripts/passo_1/processamento_imagens.py
```

---

## 6. Project Structure

```text
TCC-PROJECT/
├── dados/           # Input images and 3D models
├── scripts/         # Python scripts for each stage of the project
├── resultados/      # Generated results (images, 3D models, etc.)
├── README.md        # This file
└── requirements.txt # Project dependencies
```

---

## 7. Next Steps

- Add support for multiple images (photogrammetry)
- Build a graphical interface using Tkinter or Streamlit
- Explore more advanced techniques such as NeRF (Neural Radiance Fields)

---

## 📄 License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.

