# Super Advanced Interior Design Transformer

This repository implements an end-to-end interactive system for generating and refining interior design concepts. By leveraging state-of-the-art models including CLIP, Stable Diffusion ControlNet, and a Gradio interface, the system can:

1. **Detect Room Features:**  
   Analyze an input room image using CLIP to detect key features such as windows, sofas, tables, etc.

2. **Generate Ultra-Advanced Prompts:**  
   Dynamically build detailed prompts that include the detected room type, perspective, and additional features.

3. **Create Interior Design Variants:**  
   Use Stable Diffusion ControlNet to generate multiple design variants based on the crafted prompt and a conditioning image (derived from Canny edge detection).

4. **Iterative Refinement:**  
   Allow users to provide feedback to iteratively refine the generated designs in real time.

---

## Features

- **Room Feature Detection:**  
  Utilizes CLIP to analyze room images and extract important features.

- **Dynamic Prompt Generation:**  
  Crafts advanced, detailed prompts incorporating room type, perspective, and detected features.

- **Design Variant Generation:**  
  Produces multiple interior design variants with Stable Diffusion ControlNet.

- **Iterative Feedback Loop:**  
  Users can provide feedback to refine the designs further.

- **Interactive UI:**  
  A Gradio interface that simplifies interaction and makes the design process accessible.

---

## Installation

### Prerequisites

- Python 3.8 or higher
- A CUDA-capable GPU (recommended for faster inference)
- Required Python libraries:
  - `gradio`
  - `torch`
  - `numpy`
  - `opencv-python`
  - `transformers`
  - `diffusers`
  - `Pillow`

### Setup Steps

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/yourusername/your-repo.git
   cd your-repo
