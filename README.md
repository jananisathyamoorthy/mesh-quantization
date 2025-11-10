🧠 Mesh Quantization & Reconstruction

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1e_7VFLH-udXHiw4OhtMe5lI7tudSAlJU?usp=sharing)
![Python](https://img.shields.io/badge/Python-3.12-blue?logo=python)
![License: MIT](https://img.shields.io/badge/License-MIT-green.svg)

---

📘 Project Overview  
This project demonstrates a **3D Mesh Normalization, Quantization, and Reconstruction** pipeline built in **Google Colab**.  
It compresses and reconstructs 3D models using two normalization methods — **Min–Max** and **Unit-Sphere** — while measuring reconstruction error (**MSE** and **MAE**) for accuracy analysis.

The entire workflow is implemented using:

- ✳️ **Trimesh** — for mesh processing and I/O  
- 📊 **Plotly** — for interactive 3D visualization  
- 📈 **Matplotlib** — for error analysis plots  
- ⚙️ **NumPy** — for numerical computations  

---

🚀 Key Features  

- 🗂️ Handles `.obj`, `.ply`, `.stl`, and `.zip` mesh archives  
- 📐 Implements:  
  - **Min–Max normalization** → scales vertices to `[0, 1]`  
  - **Unit-Sphere normalization** → centers and scales mesh to fit a unit sphere  
- 🔢 Quantizes each vertex coordinate into **1024 bins**  
- 🧱 Reconstructs meshes with **minimal loss**  
- 📊 Calculates **per-axis and overall MSE/MAE**  
- 🖼️ Generates **publication-quality plots and 3D visualizations**  

---

📈 Quantization Error Analysis  

<p align="center">
  <img src="https://raw.githubusercontent.com/jananisathyamoorthy/mesh-quantization/main/errors_plot.png" width="600"/>
</p>

---

🎬 Mesh Reconstruction Animation  

<p align="center">
  <a href="https://github.com/jananisathyamoorthy/mesh-quantization/blob/main/mesh_output.mp4">
    <img src="https://raw.githubusercontent.com/jananisathyamoorthy/mesh-quantization/main/errors_plot.png" width="500"/>
  </a>
</p>

<p align="center"><i>▶️ Click the image above to watch the full 3D reconstruction video.</i></p>

---

📊 Results Summary  

| Normalization | Global MSE | Global MAE | Observations |
|----------------|------------|------------|---------------|
| **Min–Max** | Very Low | Low | High-precision reconstruction |
| **Unit-Sphere** | Low | Moderate | Scale-invariant geometry |

✅ Both methods effectively preserve geometry.  
✅ **Min–Max** normalization ensures higher numeric precision.  
✅ **Unit-Sphere** normalization offers robustness across varying scales.  

---

🗂️ Repository Structure  

mesh-quantization/
├── Mixar_ML_Assignment.ipynb # Main Google Colab notebook
├── errors_plot.png # Quantization error comparison plot
├── mesh_output.mp4 # Mesh reconstruction animation
├── reconstructed_minmax.obj # Reconstructed mesh
├── submission_package.zip # Final exported package
├── requirements.txt
├── LICENSE
└── README.md

yaml

⚙️ Run the Project in Google Colab  

1. Open the notebook directly in Colab:**  
   👉 [Launch on Colab](https://colab.research.google.com/drive/1e_7VFLH-udXHiw4OhtMe5lI7tudSAlJU?usp=sharing)

2. Execute all cells** (`Runtime → Run all`).  

3. The notebook automatically:
   - Downloads and extracts mesh data  
   - Applies Min–Max and Unit-Sphere normalization  
   - Quantizes and reconstructs mesh  
   - Exports error plots and visual results  

---

👩‍💻 Author
-- S. Janani

🎓 Final-year B.Tech CSE Student, SRM Ramapuram

💡 Passionate about UI/UX Design, Software Engineer , AI, and Data Analytics
📧 jananisathyamoorthy@example.com

📜 License
Licensed under the MIT License — free for educational and personal use.

🌟 Tags
python • colab • 3d-mesh • trimesh • ai • quantization • visualization • graphics

yaml

✅ What This Version Does
- Shows only your **error plot** (`errors_plot.png`)  
- Adds a clickable **preview** that opens the `.mp4` video  
- Removes all unused image references  
- Keeps formatting professional, dark-mode friendly, and easy to read  

---

🧩 Dependencies  

To run locally, install:
```bash
pip install trimesh meshio gdown plotly matplotlib numpy scikit-learn



