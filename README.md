Here's the updated README file with your project name, **AI Chef: A VLM makes you food**:

---

# AI Chef: A VLM Makes You Food

## Table of Contents
- [Introduction](#introduction)
- [Project Overview](#project-overview)
- [Methodology](#methodology)
  - [Fine-Tuning YOLO on Food Dataset](#fine-tuning-yolo-on-food-dataset)
  - [Recipe Generation with GPT API](#recipe-generation-with-gpt-api)
- [Results](#results)


## Introduction
Welcome to **AI Chef: A VLM Makes You Food**, a project developed as part of the Computer Vision Graduate Course at the Electrical Engineering Department, Sharif University of Technology. This project combines computer vision and natural language processing to create a unique application that detects food items in images and generates corresponding recipes.

## Project Overview
The AI Chef project leverages the power of a Visual-Language Model (VLM) to bridge the gap between visual data and language-based recipe generation. By fine-tuning a YOLO model on a food dataset and integrating the detection results with the GPT API, the project creates a seamless pipeline where food items in an image are detected and used to generate a recipe.

### Key Objectives:
- Fine-tune the YOLO model to accurately detect various food items in images.
- Use the detected food items to generate recipes via the GPT API.
- Provide a smooth and interactive user experience through a Jupyter Notebook interface.

## Methodology

### Fine-Tuning YOLO on Food Dataset
The YOLO (You Only Look Once) model, known for its real-time object detection capabilities, was fine-tuned using the UltraLytics library on a curated food dataset.

- **Dataset**: The dataset includes various food items, with annotations provided in the `data.yaml` file.
- **Model**: YOLOv5 from the UltraLytics library was chosen for its balance between accuracy and speed.
- **Training**: The model was fine-tuned through transfer learning, using pre-trained weights as a base and adapting the model to detect food items accurately.

### Recipe Generation with GPT API
Once food items are detected by the YOLO model, the next step is to generate a recipe. This is achieved through the GPT API, which processes the list of detected ingredients and generates a recipe in natural language.

- **Detection Results**: The YOLO model's output is used to extract the list of detected food items.
- **API Integration**: The GPT API generates a recipe by taking the detected ingredients as input.
- **Output**: The generated recipe is formatted and presented to the user in the notebook.



2. Follow the instructions within the notebook to fine-tune the YOLO model and generate recipes.

3. To detect food items and generate a recipe from a new image:
   - Place your image in the `data/` directory.
   - Run the detection and recipe generation cells in the notebook.

The recipe generated based on the detected food items will be displayed in the notebook output.

## Results
The fine-tuned YOLO model demonstrated high accuracy in detecting various food items, and the GPT API successfully generated coherent and relevant recipes based on these detections.

### Sample Output:
- **Detected Items**: Tomato, Cheese, Bread
- **Generated Recipe**: "Tomato and Cheese Sandwich: Place slices of tomato and cheese between bread, grill until golden brown..."


