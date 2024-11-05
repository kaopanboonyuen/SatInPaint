# 🌌 SatInPaint: Satellite Image Inpainting with Diffusion Models

Welcome to **SatInPaint**! 🚀 A cutting-edge approach for satellite image inpainting, leveraging diffusion models for efficient, high-quality restoration of missing or corrupted regions in satellite imagery. SatInPaint delivers state-of-the-art performance with reduced computational requirements, supporting both medium and high-resolution datasets such as **LANDSAT-8 (Thailand)** and **Vaihingen and Potsdam**.

## ✨ Key Features

- **⚡ Fast Inference**: Our latent-space fusion technique ensures high-quality inpainting with minimized computational cost.
- **📈 High Performance**: Achieves state-of-the-art results on both medium and high-resolution datasets.
- **💡 Novel Approach**: Combines the strengths of preconditioned and postconditioned models, without their usual trade-offs.

---

## 📂 Table of Contents

- [Installation](#installation)
- [Quick Start](#quick-start)
- [Dataset Support](#dataset-support)
- [Results](#results)
- [Citation](#citation)
- [License](#license)

---

## 🚀 Installation

To get started with SatInPaint, clone the repository and install the dependencies:

```bash
git clone https://github.com/kaopanboonyuen/SatInPaint.git
cd SatInPaint
pip install -r requirements.txt
```

> **Note**: SatInPaint requires Python 3.8+ and CUDA-compatible GPUs for best performance.

---

## 🎉 Quick Start

1. **Download Pre-trained Models**:
   - Download the pre-trained diffusion model from our release section [here](https://github.com/kaopanboonyuen/SatInPaint/releases).
   - Place the model in the `models/` directory.

2. **Run SatInPaint**:
   - To perform inpainting on an example image, simply run:
     ```bash
     python run_inpaint.py --input <path_to_input_image> --mask <path_to_mask>
     ```
   - Outputs will be saved in the `output/` folder.

3. **Configuration**:
   - SatInPaint offers several configuration options. You can adjust parameters in `config.yaml` for customized inpainting results.

---

## 🌍 Dataset Support

SatInPaint has been tested on a range of satellite datasets:
- **Medium Resolution**: Thailand’s LANDSAT-8
- **High Resolution**: Vaihingen, Potsdam

We provide scripts for pre-processing and masking satellite images for inpainting tasks. Check out the `datasets/` folder for more details.

---

## 🏆 Results

SatInPaint achieves state-of-the-art performance across different resolutions. Here’s a snapshot of our inpainting results:

| Dataset         | PSNR (↑) | SSIM (↑) |
|-----------------|----------|----------|
| LANDSAT-8       | 32.5     | 0.89     |
| Vaihingen       | 30.7     | 0.87     |
| Potsdam         | 31.3     | 0.88     |

> 📈 For detailed results and evaluation metrics, refer to my [previous work](https://kaopanboonyuen.github.io/publication/mevit-a-medium-resolution-vision-transformer/).

---

## 📄 Citation

If you use SatInPaint in your research, please cite our work:

```bibtex
@article{panboonyuen2025satinpaint,
  title={SatInPaint: Satellite Image Inpainting with Diffusion Models},
  author={Panboonyuen, Teerapong},
  year={2025}
}
```

---

## 📜 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

### 🎉 Acknowledgments

Special thanks to the **CVPR 2025** community and all contributors! 🙏

For questions or discussions, feel free to open an issue or contact us via GitHub. Happy inpainting!