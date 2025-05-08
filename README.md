# AI-Assisted Cancer Detection in EU Hospitals

## Project Overview
This project develops an advanced AI-powered diagnostic tool for cancer detection, addressing critical challenges in medical imaging across European healthcare systems. Currently, diagnostic systems for cancer detection in EU hospitals achieve only 78% accuracy, with a target of reaching 95% accuracy through AI-assisted diagnostic imaging systems. This 17% accuracy gap affects 5,631 cases, leading to delayed diagnoses, increased healthcare costs, reduced survival rates, and inefficient resource allocation.

## Key Objectives
- Increase cancer detection accuracy from 78% to 95%
- Reduce diagnostic processing time from 72 to 24 hours
- Develop a robust, generalizable AI diagnostic workflow assistant

## Repository Structure
- **EDA_Corrected.pdf**: Exploratory Data Analysis document
- **Final-Report_Group-6_LayanikaVinaySaravanan_8934459.pdf**: Comprehensive project report
- **EU_Hospitals.ipynb**: Jupyter Notebook with data analysis and visualization

## Dataset
The project utilizes the International Skin Imaging Collaboration (ISIC) 2020 dataset comprising 33,126 high-quality dermoscopic images across five main diagnostic categories:
- Nevus (45.28%)
- Basal Cell Carcinoma (15.09%)
- Melanoma (13.58%)
- Squamous Cell Carcinoma (12.08%)
- Other Lesions (13.97%)

Key challenges include extreme class imbalance (55.72:1 benign:malignant), diverse image characteristics, and the need for standardized image processing.

## Methodology
The project follows a comprehensive approach to address the accuracy gap:

### 1. Root Cause Analysis
Using the 5-Why technique and the Tree-Based Problem (TBP) framework, we identified the primary root causes of the accuracy gap:
- **Clinical Workflow Issues**: 50.0% (2,816 cases)
- **Data Analysis and AI Model Issues**: 20.0% (1,126 cases)
- **System Integration Challenges**: 17.5% (985 cases)
- **Implementation Barriers**: 12.5% (704 cases)

### 2. Countermeasures Development
Based on our analysis, we developed and evaluated several countermeasures:
- **Smart Diagnostic Workflow Assistant**: Standardizes clinical workflows
- **Enhanced AI Model System**: Improves detection for rare cancer variants
- **Seamless Integration Framework**: Addresses system integration challenges
- **Clinician Engagement Program**: Tackles implementation barriers

### 3. AI Model Implementation
We implemented an ensemble architecture combining:
- **EfficientNet-B5**: For feature extraction
- **Vision Transformer**: For contextual understanding
- **DenseNet-201**: For fine-grained classification

Additional techniques included:
- Weighted cross-entropy loss to address class imbalance
- Data augmentation for underrepresented classes
- Stratified cross-validation for robust evaluation

### 4. Statistical Validation
Our analysis included:
- Paired t-tests for diagnostic time reduction
- ANOVA for hospital tier effect on efficiency
- Chi-square tests for technological readiness effects
- Regression analysis for accuracy-time relationships

## Results
The implementation demonstrated measurable but limited progress toward addressing the accuracy gap:
- Statistical analysis confirmed a **1.00 percentage point accuracy improvement** (p<0.00001)
- This represents only **5.91% progress** toward the target 17% improvement
- Current improvement translates to approximately **332 improved diagnoses annually**
- Diagnostic time reduction from **69.05 to 23.60 hours** (65.82% reduction)
- Consistent accuracy improvement **across different hospital tiers and geographical regions**

## Challenges & Limitations
Several factors limited the achieved improvement:
- **Class imbalance**: Despite mitigation strategies, rare variants remain challenging
- **Borderline cases**: Limited capability to identify subtle differentiation factors
- **Image quality variations**: Inconsistent acquisition protocols affect performance
- **User adoption challenges**: Varying levels of acceptance across healthcare roles

## Future Enhancements
The project outlines several strategic enhancements to improve performance:
- **Advanced model architectures**: Implementing attention mechanisms for rare variant detection
- **Federated learning**: Enabling cross-border AI training while preserving patient privacy
- **Targeted data acquisition**: Addressing class imbalance with additional examples of rare variants
- **Standardized acquisition protocols**: Ensuring consistent image quality across facilities
- **Enhanced visualization tools**: Improving interpretability for healthcare professionals

Statistical modeling projects potential accuracy improvements of 8-12 percentage points over a 24-month implementation period through these enhancements.

## Prerequisites
To run the analysis, ensure you have Python 3.7+ installed along with the following dependencies:
```
pip install matplotlib pandas numpy scipy seaborn
pip install torch torchvision torchaudio efficientnet_pytorch
```

## Running the Analysis
1. Clone this repository
2. Open the EU_Hospitals.ipynb file using Jupyter Notebook
3. Run the cells to perform data analysis, visualization, and statistical testing

## Contributors
- Layanika Vinay Saravanan (ID: 8934459) - AI & ML Coordinator

## References
1. Codella, N. C. F., et al. (2019). Skin Lesion Analysis Toward Melanoma Detection.
2. Esteva, A., et al. (2021). Deep learning-enabled medical computer vision.
3. Bera, K., et al. (2019). Artificial intelligence in digital pathology.
4. Litjens, G., et al. (2017). A survey on deep learning in medical image analysis.
5. D'Andreamatteo, A., et al. (2015). Lean in healthcare: A comprehensive review.
6. Rieke, N., et al. (2020). The future of digital health with federated learning.
7. Tan, M., & Le, Q. (2019). EfficientNet: Rethinking Model Scaling for CNNs.
8. Huang, G., et al. (2017). Densely Connected Convolutional Networks.
9. Dosovitskiy, A., et al. (2021). An Image is Worth 16x16 Words: Transformers for Image Recognition at Scale.
