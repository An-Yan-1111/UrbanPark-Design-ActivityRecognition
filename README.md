# 🌳 Urban Park Design framework with activity recognition 
**Leveraging Activity Recognition and Data-Driven Spatial Planning for Sustainable Community Development**

---

## 📖 Overview
Urban parks are vital for promoting public health, ecological balance, and social unity. However, traditional park layouts often fail to adapt to real-time human activities and spatial dynamics, resulting in inefficient usage and lower community engagement.  

This research proposes a **human-centric urban park design framework** that integrates **advanced deep learning for activity recognition** and a **bio-inspired optimization algorithm for spatial planning**. The framework enables adaptive, inclusive, and efficient green space design, offering a scalable model for next-generation smart cities.

---

## 🧩 Key Contributions
- **Multiscale Vision Transformer (MViT):** Extracts multi-resolution spatiotemporal features for robust activity recognition.  
- **Spatial-Temporal Graph Convolutional Network (ST-GCN):** Models human movement and interaction patterns.  
- **Hybrid Whale-Seagull Optimization Algorithm (WSOA):**  
  - Combines exploration strategies of Whale Optimization and Seagull Optimization.  
  - Incorporates **Levy flight perturbation** for enhanced global/local search and avoiding premature convergence.  
- **Real-World Evaluation:** Achieved >95% activity recognition accuracy and up to **36% better space utilization** than baseline models.  
- **Practical Impact:** Improved **user engagement by 32%** in smart city simulations.  

---

## 📊 Datasets Used
The framework was evaluated on three complementary datasets:

1. **[UCF101](https://www.crcv.ucf.edu/data/UCF101.php)**  
   - 13,320 video clips across 101 human action classes.  
   - Benchmark dataset for real-world activity recognition.  

2. **[Stanford Drone Dataset (SDD)](http://cvgl.stanford.edu/projects/uav_data/)**  
   - 60+ hours of aerial recordings with 20,000+ human and vehicle trajectories.  
   - Provides spatial interaction data for complex outdoor environments.  

3. **[Geolife GPS Trajectory Dataset](https://www.microsoft.com/en-us/research/project/geolife-building-social-networks-using-human-location-history/)**  
   - 17,621 GPS trajectories from 178 users collected over 4 years.  
   - Captures fine-grained mobility patterns in urban spaces.  

---

## ⚙️ Methodology
1. **Data Collection & Preprocessing**  
   - Multi-source data (video, drone imagery, GPS traces).  
   - Normalization, trajectory mapping, and activity labeling.  

2. **Activity Recognition**  
   - MViT for spatiotemporal feature extraction.  
   - ST-GCN for interaction modeling.  

3. **Spatial Planning Optimization**  
   - Proposed **WSOA** algorithm assigns activity zones (walk paths, resting areas, play zones).  
   - Optimizes layout for maximum space utilization and community inclusivity.  

---

**key benefits of urban park design optimization with Activity Recognition, written in small points:**
-🧍 Human-Centric Planning – Aligns park layout with actual user behaviors and activities.
-📊 Data-Driven Decisions – Uses real-time sensor, video, and trajectory data for evidence-based design.
-🌿 Efficient Space Utilization – Maximizes functional use of walkways, play areas, and resting zones.
-🎯 Targeted Engagement – Increases community involvement by tailoring spaces to user needs.
-🔄 Adaptive Design – Supports dynamic reconfiguration of park zones as activity patterns evolve.
-🏙️ Scalable to Smart Cities – Provides a replicable model for future urban planning.
-♻️ Sustainability – Enhances ecological balance by optimizing human–environment interactions.
-🛡️ Safety & Accessibility – Improves crowd flow and reduces congestion for safer environments.
-⚙️ Optimization Performance – Outperforms traditional layouts using hybrid metaheuristic algorithms.


---

## 📂 Repository Structure
```bash
UrbanPark-Design-ActivityRecognition/
│
├── data/                # Scripts to preprocess datasets (UCF101, SDD, Geolife)
│   ├── ucf101_loader.py
│   ├── sdd_preprocess.py
│   └── geolife_parser.py
│
├── models/              # Deep learning models
│   ├── mvit_model.py
│   ├── stgcn_model.py
│   └── fusion_pipeline.py
│
├── optimization/        # Hybrid WSOA implementation
│   └── wsoa.py
│
├── experiments/         # Training and evaluation notebooks
│   ├── train_activity_recognition.ipynb
│   ├── optimize_spatial_layout.ipynb
│   └── evaluate_framework.ipynb
│
├── results/             # Results, figures, logs
│   ├── accuracy_curves.png
│   ├── utilization_comparison.png
│   └── engagement_metrics.csv
│
├── requirements.txt     # Dependencies
└── README.md            # Project documentation
