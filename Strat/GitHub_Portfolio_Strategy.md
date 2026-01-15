# GitHub Portfolio Strategy for AI Research Positions
**Anna Marie Benzon - PhD in AI**

---

## Executive Summary

This document provides a strategic analysis of your PhD projects and recommendations for presenting them on GitHub to demonstrate competence for AI Researcher and AI-related roles.

**Key Findings:**
- ✅ **4 showcase-worthy projects** identified
- ✅ **Strong technical breadth**: Medical AI, MLOps, Computer Vision, Deep Learning Theory
- ✅ **Publication-ready work**: MRI Brain Tumor Segmentation (ISBI-ready)
- ⚠️ Needs: Better documentation, code organization, and narrative framing

---

## Part 1: Project Assessment & Recommendations

### 🌟 HIGH PRIORITY - Publish These Immediately

#### 1. MRI Brain Tumor Segmentation (BraTS2020) ⭐⭐⭐⭐⭐
**Location:** `/Users/annamariebenzon/Documents/PhD in AI/MRI project`

**Why This Is Your Strongest Project:**
- Conference-ready work (ISBI template prepared)
- Complete research pipeline: data preprocessing → training → inference → radiomics analysis
- State-of-the-art architecture (nnUNet)
- 5-fold cross-validation implementation
- Advanced techniques: early stopping, TensorRT optimization, radiomics feature extraction
- Medical AI application (highly relevant for healthcare AI roles)

**What Makes It Impressive:**
- Full 369-case dataset training
- Multi-modal MRI processing (T1, T1ce, T2, FLAIR)
- Survival analysis with radiomics
- Production-ready inference pipeline
- Publication-quality visualization

**Recommended Repository Name:** `brain-tumor-segmentation-nnunet`

**Target Audience:** Medical imaging researchers, healthcare AI companies, computer vision researchers

---

#### 2. Real-time POS System with YOLOv8 on Jetson Orin ⭐⭐⭐⭐⭐
**Location:** `/Users/annamariebenzon/Documents/PhD in AI/SECOND YEAR/First Sem/AI231/MLOps Assignment/me7`

**Why This Is Exceptional:**
- End-to-end MLOps project: training → optimization → edge deployment
- Production system on embedded hardware (Jetson Orin)
- Real-time performance (<1s latency)
- Multi-modal AI: computer vision + gesture recognition + audio feedback
- TensorRT optimization for edge inference
- Professional software engineering (multi-threading, clean architecture)

**What Makes It Impressive:**
- Complete MLOps pipeline demonstrated
- Hardware-software co-optimization
- User experience design (UI, audio, gestures)
- Extensive documentation
- Performance benchmarking
- Practical application (retail automation)

**Recommended Repository Name:** `realtime-pos-yolov8-jetson`

**Target Audience:** MLOps engineers, edge AI companies, computer vision researchers, retail tech

---

#### 3. Progressive Pruning of ResNet18 on CIFAR-10 ⭐⭐⭐⭐
**Location:** `/Users/annamariebenzon/Documents/PhD in AI/SECOND YEAR/First Sem/AI231/MLOps Assignment/Pruned ResNet18 for CIFAR10`

**Why This Is Strong:**
- Model compression research (relevant for edge deployment)
- Systematic experimental methodology
- Comparison of pruning strategies (structured vs. unstructured)
- Comprehensive analysis with visualization
- Well-documented codebase
- Research question: "How many pruning cycles before degradation?"

**What Makes It Impressive:**
- Original research contribution
- Scientific rigor (multiple pruning methods, performance tracking)
- Practical significance (model efficiency)
- Clean code structure
- Publication-quality analysis

**Recommended Repository Name:** `iterative-pruning-resnet18-cifar10`

**Target Audience:** ML efficiency researchers, edge AI engineers, model optimization specialists

---

### ✅ MEDIUM PRIORITY - Good Supporting Projects

#### 4. Sleep Apnea Detection from ECG Signals ⭐⭐⭐⭐
**Location:** `/Users/annamariebenzon/Documents/PhD in AI/FIRST YEAR/FIRST TERM/AI 201/Miniproject`

**Why This Is Valuable:**
- Medical AI application (different from brain imaging)
- Signal processing + machine learning
- Feature engineering from physiological signals
- SMOTE for class imbalance
- Cross-validation with comprehensive evaluation

**What Makes It Useful:**
- Demonstrates versatility (imaging + signals)
- Healthcare domain knowledge
- Classical ML expertise (Random Forest, feature selection)
- Complete ML pipeline

**Recommended Repository Name:** `sleep-apnea-detection-ecg`

**Target Audience:** Healthcare AI, biomedical signal processing researchers

---

### ⚠️ LOW PRIORITY - Optional/Archive

#### 5. AlexNet Implementation (MLOps Assignment)
**Status:** Archive or include as part of MLOps portfolio
**Reason:** Educational exercise, not novel contribution

#### 6. MNIST Classification
**Status:** Archive
**Reason:** Too basic for PhD-level demonstration

#### 7. AI 301 Computational Learning Theory
**Status:** Do NOT publish
**Reason:** Coursework exercises, not original research. Theoretical exercises are better demonstrated through applications.

---

## Part 2: Repository Organization Strategy

### A. Individual Repository Structure

Each project should follow this template:

```
project-name/
├── README.md                 # Compelling project overview
├── INSTALLATION.md          # Setup instructions
├── docs/
│   ├── methodology.md       # Technical approach
│   ├── results.md          # Experimental results
│   └── architecture.md     # System design (if applicable)
├── src/                    # Source code
│   ├── models/
│   ├── data/
│   ├── training/
│   └── inference/
├── notebooks/              # Jupyter notebooks for exploration
├── experiments/            # Experiment configs and logs
├── results/               # Visualizations, metrics, outputs
├── requirements.txt       # Dependencies
├── setup.py              # Package setup (if applicable)
├── .gitignore
└── LICENSE               # MIT or Apache 2.0 recommended
```

### B. README.md Template for Each Project

```markdown
# Project Title

![Demo Image/GIF]

**One-sentence description of what this does and why it matters**

[![Python 3.8+](badge)]
[![License: MIT](badge)]
[![Framework](badge)]

## Overview

A concise paragraph explaining:
- The problem you're solving
- Your approach
- Key results/achievements

## Key Features

- 🚀 **Feature 1**: Brief description
- 🎯 **Feature 2**: Brief description
- 📊 **Feature 3**: Brief description

## Results

### Quantitative Results
- Metric 1: XX.X%
- Metric 2: XX.X ms
- Metric 3: XX.X

### Visualizations
![Result 1]
![Result 2]

## Quick Start

```bash
# Installation
pip install -r requirements.txt

# Run
python main.py
```

## Methodology

Brief technical overview with links to detailed docs/

## Project Structure

```
src/
├── models/
├── training/
└── inference/
```

## Technologies Used

- PyTorch / TensorFlow
- nnUNet / YOLO / etc.
- Other key libraries

## Citation

If you use this work, please cite:
```bibtex
@misc{benzon2024project,
  author = {Benzon, Anna Marie},
  title = {Project Title},
  year = {2024},
  url = {https://github.com/...}
}
```

## License

MIT License

## Contact

Anna Marie Benzon - [LinkedIn](link) | [Email](email)
```

---

## Part 3: Specific Strategies for Each Project

### 🧠 Project 1: Brain Tumor Segmentation

**Repository Name:** `brain-tumor-segmentation-nnunet`

**Key Documentation to Create:**

1. **README.md** - Focus on:
   - Clinical significance (brain tumor diagnosis)
   - nnUNet architecture explanation
   - 5-fold CV results with Dice scores
   - Radiomics integration
   - Sample segmentation visualizations

2. **docs/preprocessing.md** - Explain:
   - Multi-modal MRI alignment
   - Intensity normalization
   - Data augmentation strategies

3. **docs/training.md** - Detail:
   - nnUNet configuration
   - 5-fold cross-validation setup
   - Early stopping criteria
   - Training time and resources

4. **docs/radiomics.md** - Describe:
   - Feature extraction methodology
   - PyRadiomics integration
   - Survival analysis approach

**What to Include:**
```
brain-tumor-segmentation-nnunet/
├── README.md
├── INSTALLATION.md
├── docs/
│   ├── preprocessing.md
│   ├── training.md
│   ├── radiomics.md
│   └── results.md
├── src/
│   ├── preprocessing/
│   │   ├── relabel_masks.py
│   │   └── create_dataset.py
│   ├── training/
│   │   ├── nnunet_trainer.py
│   │   └── early_stopping.py
│   ├── inference/
│   │   └── predict.py
│   └── radiomics/
│       ├── extract_features.py
│       └── survival_analysis.py
├── notebooks/
│   ├── 01_data_exploration.ipynb
│   ├── 02_training_visualization.ipynb
│   └── 03_results_analysis.ipynb
├── configs/
│   └── dataset.json
├── results/
│   ├── segmentation_samples/
│   ├── dice_scores.csv
│   └── radiomics_features.csv
├── requirements.txt
└── LICENSE
```

**Visualizations to Create:**
- Axial, sagittal, coronal views of segmentations
- Ground truth vs. prediction comparisons
- Dice score distributions across folds
- Radiomics feature importance plots
- Training curves (loss, Dice over epochs)

**Narrative to Emphasize:**
> "Implemented state-of-the-art nnUNet for multi-modal brain tumor segmentation on BraTS2020 dataset, achieving competitive Dice scores across 5-fold cross-validation. Extended the pipeline with PyRadiomics feature extraction for downstream survival analysis, demonstrating end-to-end research capability from segmentation to clinical outcome prediction."

---

### 🛒 Project 2: Real-time POS System

**Repository Name:** `realtime-pos-yolov8-jetson`

**Key Documentation to Create:**

1. **README.md** - Highlight:
   - End-to-end MLOps pipeline
   - Real-time performance (<1s latency)
   - Edge deployment on Jetson Orin
   - Multi-modal interaction (vision + gesture + audio)
   - Demo video/GIF

2. **docs/architecture.md** - Detail:
   - System architecture diagram
   - Multi-threading design
   - TensorRT optimization
   - Performance benchmarks

3. **docs/deployment.md** - Explain:
   - Jetson Orin setup
   - Model conversion to TensorRT
   - Performance tuning

**What to Include:**
```
realtime-pos-yolov8-jetson/
├── README.md
├── INSTALLATION.md
├── docs/
│   ├── architecture.md
│   ├── deployment.md
│   ├── training.md
│   └── performance.md
├── src/
│   ├── pos_system.py
│   ├── object_detector.py
│   ├── gesture_detector.py
│   ├── audio_manager.py
│   └── pos_ui.py
├── training/
│   ├── train_yolo.py
│   └── data/
├── models/
│   └── best.pt
├── configs/
│   └── products.json
├── demo/
│   ├── demo.gif
│   └── screenshots/
├── requirements.txt
└── LICENSE
```

**Visualizations to Create:**
- System architecture diagram
- Demo GIF showing full workflow
- Performance comparison (TensorRT vs. PyTorch)
- Detection examples with bounding boxes
- Gesture recognition visualization

**Narrative to Emphasize:**
> "Developed production-ready point-of-sale system with real-time object detection (YOLOv8) and gesture control, optimized for NVIDIA Jetson Orin edge deployment. Achieved <1s latency through TensorRT optimization and multi-threaded architecture. Demonstrates complete MLOps pipeline: data collection → model training → optimization → edge deployment → user experience design."

---

### 📉 Project 3: Progressive Pruning

**Repository Name:** `iterative-pruning-resnet18-cifar10`

**Key Documentation to Create:**

1. **README.md** - Focus on:
   - Research question clearly stated
   - Comparison of structured vs. unstructured pruning
   - Performance degradation analysis
   - Compression ratios achieved

2. **docs/methodology.md** - Detail:
   - Pruning algorithms (L2-norm, magnitude-based)
   - Fine-tuning protocol
   - Evaluation metrics

3. **docs/results.md** - Present:
   - Degradation curves
   - Compression vs. accuracy trade-offs
   - Comparative analysis

**What to Include:**
```
iterative-pruning-resnet18-cifar10/
├── README.md
├── docs/
│   ├── methodology.md
│   ├── results.md
│   └── analysis.md
├── src/
│   ├── model.py
│   ├── pruning.py
│   ├── trainer.py
│   └── data_loader.py
├── experiments/
│   ├── structured_pruning/
│   └── unstructured_pruning/
├── results/
│   ├── plots/
│   └── metrics/
├── notebooks/
│   └── analysis.ipynb
├── requirements.txt
└── LICENSE
```

**Visualizations to Create:**
- Accuracy vs. pruning cycles
- Model size reduction over cycles
- Structured vs. unstructured comparison
- Degradation point identification

**Narrative to Emphasize:**
> "Systematic investigation of iterative pruning strategies for neural network compression, comparing structured and unstructured approaches. Identified optimal compression ratios before performance degradation, achieving 10-20x compression for unstructured pruning with minimal accuracy loss. Demonstrates understanding of model efficiency critical for edge deployment."

---

### 🫀 Project 4: Sleep Apnea Detection

**Repository Name:** `sleep-apnea-detection-ecg`

**Key Documentation to Create:**

1. **README.md** - Emphasize:
   - Clinical significance (sleep disorder diagnosis)
   - Feature engineering from ECG signals
   - Class imbalance handling (SMOTE)
   - Cross-validation results

2. **docs/features.md** - Explain:
   - HRV features
   - Statistical features
   - Feature selection rationale

**What to Include:**
```
sleep-apnea-detection-ecg/
├── README.md
├── docs/
│   ├── features.md
│   └── methodology.md
├── src/
│   ├── preprocessing.py
│   ├── feature_extraction.py
│   └── classifier.py
├── notebooks/
│   └── analysis.ipynb
├── data/
│   └── README.md (explain how to get APNEA-ECG dataset)
├── results/
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── feature_importance.png
├── requirements.txt
└── LICENSE
```

**Narrative to Emphasize:**
> "Developed machine learning pipeline for automated sleep apnea detection from single-lead ECG signals using the APNEA-ECG database. Engineered HRV and statistical features, addressed class imbalance with SMOTE, and achieved strong classification performance with Random Forest. Demonstrates expertise in biomedical signal processing and clinical AI applications."

---

## Part 4: GitHub Profile Optimization

### A. Profile README (Create a Special Repository)

Create a repository named: `your-username/your-username`

Example `README.md`:

```markdown
# Anna Marie Benzon

**PhD Candidate in AI | Medical Imaging & Computer Vision Researcher**

🔬 Developing AI systems for healthcare and edge computing
🧠 Specializations: Medical Image Segmentation, MLOps, Model Optimization
🎯 Passionate about bridging research and production

## 🚀 Featured Projects

### 🧠 [Brain Tumor Segmentation with nnUNet](link)
State-of-the-art segmentation on BraTS2020 with radiomics integration
- Multi-modal MRI processing
- 5-fold cross-validation
- Survival analysis

### 🛒 [Real-time POS System on Jetson Orin](link)
Production-ready edge AI system with YOLOv8
- <1s latency on embedded hardware
- TensorRT optimization
- Multi-modal interaction

### 📉 [Progressive Neural Network Pruning](link)
Systematic study of model compression strategies
- 10-20x compression ratios
- Structured vs. unstructured comparison

## 🛠️ Technical Skills

**AI/ML:** PyTorch, TensorFlow, nnUNet, YOLO, Scikit-learn, OpenCV
**MLOps:** TensorRT, ONNX, Docker, Jetson SDK
**Medical Imaging:** PyRadiomics, SimpleITK, MONAI
**Languages:** Python, CUDA, C++

## 📊 GitHub Stats

![Your GitHub stats]

## 📫 Connect

- 🔗 LinkedIn: [link]
- 📧 Email: [email]
- 🎓 Institution: [PhD program]
```

### B. Repository Topics/Tags

For each repository, add relevant tags:

**Brain Tumor Segmentation:**
- `medical-imaging`
- `deep-learning`
- `segmentation`
- `nnunet`
- `pytorch`
- `brain-tumor`
- `radiomics`
- `mri`

**POS System:**
- `yolov8`
- `jetson-orin`
- `edge-ai`
- `tensorrt`
- `mlops`
- `computer-vision`
- `real-time`
- `object-detection`

**Pruning:**
- `model-compression`
- `neural-network-pruning`
- `resnet`
- `cifar10`
- `model-optimization`
- `edge-ai`

### C. Pin Your Best Repositories

Pin these 4-6 repositories on your GitHub profile:
1. Brain Tumor Segmentation
2. Real-time POS System
3. Progressive Pruning
4. Sleep Apnea Detection
5. (Optional) A theory/algorithm repository if you create one
6. (Optional) Your profile README repository

---

## Part 5: Documentation Best Practices

### A. README Quality Checklist

For each project, ensure your README has:

- [ ] Clear, concise title
- [ ] Badges (Python version, license, framework)
- [ ] Demo image/GIF in first 2 screens
- [ ] One-sentence hook ("What does this do?")
- [ ] Key features (3-5 bullet points)
- [ ] Results section with metrics
- [ ] Quick start (< 5 steps to run)
- [ ] Technologies used
- [ ] License
- [ ] Contact information
- [ ] Citation (for research projects)

### B. Code Quality Standards

Before publishing:

- [ ] Remove personal paths (use relative paths)
- [ ] Remove credentials, API keys
- [ ] Clean up commented-out code
- [ ] Add docstrings to all functions/classes
- [ ] Include type hints (Python 3.8+)
- [ ] Format code (black, autopep8)
- [ ] Add .gitignore (Python template)
- [ ] Include requirements.txt with versions
- [ ] Test that installation instructions work

### C. Visual Documentation

Create these visualizations for each project:

**Required:**
- Architecture diagram (if applicable)
- Results plots/charts
- Example inputs/outputs

**Nice to Have:**
- Demo GIF/video
- Training curves
- Comparison tables
- Performance benchmarks

**Tools:**
- Diagrams: draw.io, Lucidchart, mermaid.js
- Plots: matplotlib, seaborn, plotly
- GIFs: screen recording → ezgif.com

---

## Part 6: Pre-Publication Checklist

### For Each Repository:

#### 1. Clean Up
- [ ] Remove all personal/absolute paths
- [ ] Remove any sensitive data
- [ ] Remove duplicate/unused files
- [ ] Organize into logical structure
- [ ] Create .gitignore

#### 2. Documentation
- [ ] Write comprehensive README.md
- [ ] Create INSTALLATION.md
- [ ] Add docstrings to code
- [ ] Create docs/ folder with detailed explanations
- [ ] Add LICENSE file

#### 3. Code Quality
- [ ] Refactor into modular functions
- [ ] Add command-line interfaces
- [ ] Create requirements.txt
- [ ] Test installation process
- [ ] Verify all scripts run

#### 4. Visuals
- [ ] Create architecture diagrams
- [ ] Generate result visualizations
- [ ] Create demo GIF/screenshots
- [ ] Add plots to README

#### 5. Finalize
- [ ] Add repository topics/tags
- [ ] Write detailed commit messages
- [ ] Create releases (v1.0.0)
- [ ] Pin to profile (if top project)
- [ ] Share on LinkedIn

---

## Part 7: Publication Timeline

### Week 1: Preparation
- Clean up all 4 projects locally
- Create visualizations
- Write documentation drafts

### Week 2: Brain Tumor Segmentation
- Organize repository structure
- Write README and docs
- Create demo visualizations
- Publish repository
- Share on LinkedIn

### Week 3: POS System
- Organize repository structure
- Create architecture diagram
- Record demo video
- Publish repository
- Share on LinkedIn

### Week 4: Pruning & Sleep Apnea
- Organize both repositories
- Create visualizations
- Publish repositories
- Update profile README

### Ongoing:
- Respond to issues/questions
- Keep documentation updated
- Add new results as research progresses

---

## Part 8: Career Positioning Strategy

### A. Narrative Framework

When describing yourself on LinkedIn/CV, structure around these 4 projects:

**Medical AI Expertise:**
> "Developed state-of-the-art brain tumor segmentation pipeline using nnUNet on BraTS2020 dataset, with radiomics integration for survival analysis. Also created automated sleep apnea detection from ECG signals, demonstrating breadth in medical AI applications across imaging and physiological signals."

**MLOps & Production Systems:**
> "Built production-ready real-time object detection system deployed on NVIDIA Jetson Orin with <1s latency, showcasing complete MLOps pipeline from training through edge optimization and deployment."

**AI Efficiency & Optimization:**
> "Conducted systematic research on neural network compression, comparing pruning strategies and achieving 10-20x model compression while maintaining accuracy—critical for edge AI deployment."

### B. Skills Demonstrated Across Projects

| Skill Category | Projects Demonstrating This |
|----------------|----------------------------|
| Medical Imaging AI | Brain Tumor Segmentation, Sleep Apnea |
| Computer Vision | POS System, Brain Tumor Segmentation |
| MLOps | POS System, Brain Tumor Segmentation |
| Edge AI | POS System, Pruning Research |
| Signal Processing | Sleep Apnea Detection |
| Deep Learning | All projects |
| Model Optimization | Pruning Research, POS System (TensorRT) |
| Research Methodology | Brain Tumor Segmentation, Pruning |
| Production Engineering | POS System |
| Healthcare Applications | Brain Tumor, Sleep Apnea |

### C. Target Job Roles

These projects position you for:

**Primary Targets:**
1. Medical AI Researcher (healthcare companies, research labs)
2. Computer Vision Engineer (autonomous vehicles, robotics)
3. MLOps Engineer (tech companies, AI platforms)
4. AI Research Scientist (research labs, PhD continuation)

**Secondary Targets:**
5. Deep Learning Engineer
6. Edge AI Engineer
7. AI Product Manager (technical background)

---

## Part 9: Advanced Tips

### A. Creating Compelling Demos

**For Brain Tumor Segmentation:**
- Create side-by-side comparison video (MRI slice → segmentation overlay)
- Use medical visualization libraries (nilearn, matplotlib with medical colormaps)
- Show 3D renderings of tumors

**For POS System:**
- Record full workflow demo (gesture start → item scan → gesture end)
- Create speed comparison (before/after TensorRT)
- Show multi-threading performance

### B. Blogging About Your Work

Consider writing blog posts on Medium/personal blog:
- "Building a Real-time POS System with YOLOv8 on Jetson Orin"
- "State-of-the-art Brain Tumor Segmentation with nnUNet"
- "How Many Times Can You Prune a Neural Network?"

Link these in your repository READMEs.

### C. Engagement Strategy

**On GitHub:**
- Star related repositories in your field
- Comment on issues in tools you use (nnUNet, YOLO)
- Create GitHub Actions for CI/CD (advanced)

**On LinkedIn:**
- Share each repository launch with:
  - Visual (demo GIF or results)
  - Brief explanation (3-4 sentences)
  - Link to repository
  - Relevant hashtags (#MedicalAI #ComputerVision #MLOps)

**At Conferences:**
- Prepare poster/presentation from MRI project
- Submit to ISBI or similar conferences
- Reference GitHub repository in submissions

---

## Part 10: Long-term Maintenance

### A. Keep Projects Active

- Respond to issues within 48 hours
- Update documentation based on questions
- Add "Contributions welcome" if open to PRs
- Create GitHub Actions for automated testing
- Regular dependency updates

### B. Expand Projects Over Time

**Brain Tumor Segmentation:**
- Add more architectures (U-Net, Attention U-Net)
- Ensemble methods
- Uncertainty quantification
- External validation on different datasets

**POS System:**
- Add more YOLO versions comparison
- Support for different Jetson platforms
- Multi-camera support
- Cloud integration

**Pruning:**
- Add more pruning methods
- Different architectures
- Lottery ticket hypothesis experiments

### C. Track Impact

Monitor:
- GitHub stars, forks, watchers
- LinkedIn post engagement
- Job interview mentions
- Collaboration requests

---

## Conclusion

**Immediate Actions (Priority Order):**

1. **This Week:** Clean up and publish Brain Tumor Segmentation project
   - This is your strongest, most research-ready project
   - Creates immediate credibility

2. **Next Week:** Publish POS System project
   - Demonstrates production/MLOps skills
   - Highly visual and engaging

3. **Following Weeks:** Publish Pruning and Sleep Apnea projects
   - Round out your portfolio
   - Show breadth of expertise

4. **Ongoing:** Optimize GitHub profile, create profile README, maintain projects

**Expected Outcome:**

A compelling GitHub portfolio that demonstrates:
- ✅ Research capability (publication-ready work)
- ✅ Production engineering (edge deployment)
- ✅ Medical AI expertise (multiple applications)
- ✅ MLOps proficiency (training → deployment)
- ✅ Theoretical understanding (pruning research)
- ✅ Software engineering (clean, documented code)

This positions you competitively for AI Research Scientist, Medical AI Researcher, Computer Vision Engineer, and MLOps Engineer roles.

---

**Next Steps:**
1. Review this document
2. Start with Brain Tumor Segmentation cleanup
3. Create repository templates locally
4. Begin documentation writing
5. Schedule publication dates

Good luck with your GitHub portfolio! 🚀
