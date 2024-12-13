# Mars Terrain Semantic Segmentation

## Project Overview
A cutting-edge deep learning solution for semantic segmentation of Mars terrain, developed as part of the 2024-2025 Artificial Neural Networks and Deep Learning course. The project tackles the complex challenge of automatically segmenting and understanding Martian surface topography using advanced computer vision techniques.

## Team Bergers
- **Members**:
  - Francesco Palma
  - Francesco Pellegrini
  - Luigi Raggi

## Challenge Specifications
- **Platform**: Kaggle Semantic Segmentation Challenge
- **Objective**: Develop a model to accurately segment Mars terrain images
- **Unique Constraint**: No pretrained models allowed - training from scratch

## Technological Innovation: MarsSeg Architecture

### Model Design Rationale
The MarsSeg framework was meticulously crafted to address the unique challenges of Martian terrain segmentation:
- Specialized for extraterrestrial ground types
- Optimized for small, complex datasets
- Designed to handle minimal inter-class feature differences

### Architectural Highlights
- **Encoder-Decoder Structure**
- **Feature Enhancement Connections**:
  - Mini-ASPP (Multi-scale Context Extraction)
  - PSA (Pixel Spatial Attention)
  - SPPM (Shallow and Mid-level Feature Enhancement)

## Advanced Methodology

### Data Augmentation Strategy
- **Approach**: Offline augmentation
- **Techniques**:
  - Horizontal image flipping
  - Mask dropout
  - Targeted oversampling of underrepresented classes
- **Dataset Expansion**: Doubled original dataset size

### Optimization Techniques
- **Optimizer**: AdamW
- **Loss Function**: Custom Sparse Categorical Crossentropy
  - Ignores background pixels
  - Tailored to improve mean IoU
- **Learning Rate**: 1e-4 with adaptive reduction

## Performance Breakdown

### Model Comparative Analysis
| Model | Mean IoU |
|-------|----------|
| SegFormer | 0.53 |
| UNet | 0.63 |
| DeepLabV3 | 0.68 |
| **MarsSeg** | **0.69** |

### Granular Performance Metrics
| Terrain Class | IoU Score |
|--------------|-----------|
| Class 1 | 0.8701 |
| Class 2 | 0.8064 |
| Class 3 | 0.8755 |
| "Big Rock" Class | 0.2032 |

## Research Challenges Addressed
- Extremely limited annotated Martian surface data
- Highly imbalanced dataset
- Complex, variable terrain features
- Minimal distinguishing inter-class characteristics

## Innovative Techniques Explored
- Custom segmentation architectures
- Advanced loss function engineering
- Sophisticated data augmentation
- Class imbalance mitigation strategies

## Limitations and Insights
- Identified potential labeling inconsistencies in dataset
- Discovered sensitivity of model to augmentation techniques
- Highlighted challenges in segmenting underrepresented terrain classes

## Potential Future Improvements
- Enhanced feature extraction for minority classes
- Advanced attention mechanisms
- More nuanced augmentation strategies
- Addressing "big rock" class segmentation challenges

## Technical Ecosystem
- **Frameworks**: TensorFlow, Keras
- **Augmentation Library**: Albumentations
- **Custom Deep Learning Components**

## Research Impact
Demonstrates innovative approach to semantic segmentation in challenging, data-limited scenarios, with potential applications in:
- Planetary exploration
- Autonomous robotic navigation
- Geological analysis of extraterrestrial terrain

## Acknowledgments
Gratitude to course instructors, Kaggle platform, and the spirit of scientific exploration.

---

*Artificial Neural Networks and Deep Learning Course Project*
*December 2024*
