# The-Hitchhiker-s-Guide-to-PyTorch-Multi-Layer-Perceptron

This project involves building and training a neural network using PyTorch to classify handwritten digits from the popular MNIST dataset.

 🗃️ Dataset: MNIST
The MNIST dataset is a benchmark dataset in the field of machine learning, consisting of:

- 60,000 training images
- 10,000 testing images
- Grayscale handwritten digits from 0–9
- Each image is 28x28 pixels

🔧 Technologies Used
- Python
- PyTorch: Deep learning framework
- Torchvision: Dataset and transform utilities
- NumPy, Matplotlib: Optional visualization & data utilities

⚙️ Project Workflow
🛠️ Data Preparation
- Downloaded and normalized MNIST images using transforms.Normalize().
- Used DataLoader with SubsetRandomSampler for batching and shuffling.

🧠 Model Architecture
- A custom fully connected feedforward neural network (FNN) built using torch.nn:
- Input Layer: 784 nodes (28x28)
- Hidden Layers: Two hidden layers with ReLU activations
- Output Layer: 10 nodes (for digits 0–9)

📈 Training Process
- Optimizer: Adam
- Loss Function: CrossEntropyLoss
- Device: Trained using CUDA GPU if available, otherwise CPU
- Epochs: 20
- Batch size: 64

✅ Evaluation
- Validation during training using a held-out validation set
- Final testing on the MNIST test set

🔍 Results
- The model achieves high accuracy (>97%) on the MNIST test set
- Demonstrates successful use of GPU acceleration and PyTorch pipelines
- Shows ability to generalize on unseen digit images
