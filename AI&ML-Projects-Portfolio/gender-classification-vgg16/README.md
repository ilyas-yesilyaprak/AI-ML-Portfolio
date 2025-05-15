# Gender Classification with VGG-16

This project performs binary gender classification using the CelebA dataset and transfer learning with a pretrained VGG-16 model.

## 📊 Dataset
- **CelebA30k**: A filtered subset of the CelebA dataset with 30,000+ labeled celebrity face images.
- **Split**: 80% Training, 10% Validation, 10% Test
- **Stratified** sampling to preserve gender distribution

## 🧠 Model & Architecture
- **Base Model**: VGG-16 pretrained on ImageNet
- **Input Size**: 224x224 RGB images
- **Fine-tuning**: Experiments with frozen layers vs fine-tuning last convolution block

## 🔁 Experiment Settings
- **Optimizer**: Adam
- **Loss Function**: Binary Cross Entropy
- **Learning Rates Tested**: 0.001, 0.0001
- **Fine-tuning**: ON and OFF tested
- **Epochs**: 10 per experiment
- **Accelerator**: Google Colab T4 GPU (runtime)

## 🧪 Results
| Experiment | Learning Rate | Fine-tuning | Test Accuracy |
|------------|----------------|-------------|----------------|
| 1          | 0.001          | No          | 93.70%         |
| 2          | 0.0001         | No          | 94.73%         |
| 3          | 0.001          | Yes         | 93.63%         |
| 4          | 0.0001         | Yes         | **96.23%**     |

## 📈 Evaluation
- Accuracy Score
- Confusion Matrix
- Training & Validation Loss Curves (via Matplotlib)

## 🛠️ Tech Stack
Python, PyTorch, Torchvision, Google Colab, Matplotlib, Pandas

## 🚀 How to Run
1. Open the notebook in Google Colab
2. Mount Google Drive and load the dataset
3. Run the full notebook to train and evaluate the four models
