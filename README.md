# Technology Mining the Evolution of Humanoid Robotics: A BERT and DeepSeek based Framework for Mapping Innovation Trajectories across Global Patent Grants and Open-Source Repositories

Authors: Usharani Hareesh Govindarajan<sup>1</sup>, Yuecheng Hong<sup>2</sup>, Cristian Mejia<sup>1</sup>, Gagan Narang<sup>3</sup>  
Affiliations:  
<sup>1</sup>Institute for Future Initiatives, University of Tokyo, Tokyo, Japan  
 <sup>2</sup>School of Management, Harbin Institute of Technology, Harbin, China  
 <sup>3</sup>Department of Information Engineering, Università Politecnica delle Marche, Ancona, Italy  

---

## 🧠 Overview

Humanoid robotics is rapidly advancing, driven by the convergence of multimodal AI, advanced mechatronics, and human-robot interaction technologies. This project proposes a hybrid technology mining framework to compare and analyze innovation trajectories across **closed-source (patents)** and **open-source (GitHub)** ecosystems.

We employ:
- **BERTopic** for topic extraction from patent abstracts and GitHub+Huging Face README files.
- **DeepSeek-V3** for explainable reclassification into technological functions.

The study reveals distinct patterns in innovation models, demonstrating how proprietary and collaborative ecosystems drive innovation differently in the humanoid robotics domain.

---

## 📁 Code Structure

The repository includes the following core notebooks:

### `1. EDA.ipynb`
- Initial exploratory data analysis (EDA) on the retrieved patent and GitHub+Hugging Face datasets.
- Includes preprocessing, filtering based on quality metrics (e.g., stars > 10 on GitHub), and statistical visualization of trends over time.
- Key visualizations: publication counts by year, geospatial trends, citation/star distribution.

### `2. BERT+DeepSeekV3.ipynb`
- Implements a BERTopic pipeline to extract semantically coherent clusters of innovation topics from patent and GitHub corpora.
- Uses DeepSeek-V3 for reclassification of extracted topics into four major technical categories: **Actuators, Brains, Sensors, Batteries**.
- Includes explainable AI integration and results interpretation using both intrinsic and extrinsic validation.

---

## 📊 Key Contributions

- **Novel comparative framework**: Enables cross-source mining between structured (patent) and unstructured (open-source) data.
- **Temporal & geographic innovation mapping**: Shows bursts of development aligned with milestones in AI and robotics (e.g., Atlas launch, GPT/ROS releases).
- **Open-source vs. Patent divergence**: 
  - Patents: hardware, control circuits, mobility, protected innovations.
  - GitHub+Hugging Face: cognitive models, simulations, software middleware.

---

## 🚀 Getting Started

To reproduce the results:

1. Clone the repository
2. Ensure the required dependencies from `requirements.txt` are installed
3. Run the notebooks in order:
   - `1. EDA.ipynb`
   - `2. BERT+DeepSeekV3.ipynb`

---

## 📌 Data Sources

- **Patents**: Retrieved via IncoPat covering 2010–2024 (5,612 entries).
- **Open-source**: GitHub repositories matching keywords “humanoid robot” (2,429 entries initially, filtered to 148 high-quality repos).
- **Hugging Face**: Supplementary LLM metadata.

---

## 📈 Results Highlights

- **133 patent topics** and **15 GitHub topics** extracted.
- Patent innovation dominated by actuator design.
- GitHub and Hugging Face innovation led by AI models and simulation platforms.
- Validated using semantic alignment with IPC/CPC classifications, showing >81% alignment.

---

## 📜 License

This is open-source software made available under the [MIT License](LICENSE).  
Copyright © 2025 Usharani Hareesh Govindarajan, Yuecheng Hong, Cristian Mejia, and Gagan Narang.

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, subject to the following conditions:

> The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED...

---

## 📄 Citation

If you use this work, please cite:

```
@article{govindarajan2025techmining,
  title={Technology Mining the Evolution of Humanoid Robotics},
  author={Govindarajan, Usharani Hareesh and Hong, Yuecheng and Mejia, Cristian and Narang, Gagan},
  journal={Preprint under review},
  year={2025}
}
```

---

## 🔗 Related Resources
- [BERTopic Documentation](https://maartengr.github.io/BERTopic/)
- [DeepSeek-V3 Technical Report](https://arxiv.org/abs/2412.19437)
