# FrameForge – AI-Powered Storyboard Generation Platform

**An AI-driven platform for transforming textual narratives into cinematic visual storyboards using Large Language Models and Generative AI.**

## Overview

FrameForge is an AI-powered storyboard generation platform that transforms creative story descriptions into structured cinematic scenes and corresponding visual frames.

The application integrates Google's Gemini API for intelligent story decomposition and prompt generation with Stable Diffusion for cinematic image synthesis. It also incorporates custom Low-Rank Adaptation (LoRA) training to improve character consistency across generated scenes.

Built using Python, Streamlit, PyTorch, and Hugging Face Diffusers, the platform provides an integrated workflow for AI-assisted visual storytelling and storyboard creation.

## Key Features

### 1. AI-Powered Story Generation
- Generate structured storyboards using Google Gemini.
- Convert natural language descriptions into individual cinematic scenes.
- Automatically generate scene descriptions and image-generation prompts.
- Support multiple storytelling genres.
- Generate camera shot descriptions, visual moods, and scene compositions.

### 2. Custom Character Training with LoRA
- Train custom character representations using reference images.
- Configure character trigger tokens.
- Fine-tune Stable Diffusion using Low-Rank Adaptation.
- Export trained model weights in Safetensors format.
- Reuse trained character models during storyboard generation.

### 3. Generative Image Synthesis
- Generate cinematic images using Stable Diffusion 1.5.
- Convert AI-generated scene descriptions into visual compositions.
- Support different image resolutions and aspect ratios.
- Configure inference parameters for image generation.
- Integrate custom LoRA weights into the generation pipeline.

### 4. Character Consistency
- Integrate custom-trained LoRA models into image generation.
- Configure LoRA strength during inference.
- Incorporate character-specific trigger tokens.
- Refine prompts based on scene composition and camera perspective.

### 5. Image Enhancement
- Integrate GFPGAN for facial restoration.
- Support optional image-to-image refinement.
- Improve facial details and visual quality.
- Configure enhancement options within the generation workflow.

### 6. Interactive Application
- Streamlit-based interactive interface.
- Separate workflows for character training and storyboard generation.
- Configurable scene count and image resolution.
- Training logs and generation progress.
- Preview and download generated storyboard frames.

## Technology Stack

| Category | Technologies |
|---|---|
| Programming | Python |
| Application Framework | Streamlit |
| Large Language Model | Google Gemini API |
| Image Generation | Stable Diffusion 1.5 |
| Deep Learning | PyTorch |
| Model Fine-tuning | LoRA |
| Model Framework | Hugging Face Diffusers |
| Training Framework | Kohya SS |
| Image Enhancement | GFPGAN |
| Image Processing | OpenCV, Pillow, NumPy |
| Model Serialization | Safetensors |
| Development Environment | Google Colab |
| Application Access | Ngrok |

## System Architecture

```text
                 USER INPUT
                     |
                     v
          STORY DESCRIPTION
                     |
                     v
           GOOGLE GEMINI API
                     |
                     v
          STORY DECOMPOSITION
                     |
                     v
           CINEMATIC SCENE
              GENERATION
                     |
                     v
            PROMPT ENGINEERING
                     |
                     v
          CUSTOM CHARACTER LoRA
              INTEGRATION
                     |
                     v
            STABLE DIFFUSION
               PIPELINE
                     |
                     v
             IMAGE SYNTHESIS
                     |
                     v
           IMAGE ENHANCEMENT
                     |
                     v
           STORYBOARD OUTPUT
                     |
                     v
          FRAME PREVIEW / EXPORT
```

## Application Workflow

1. **Story Input:** Users provide a story title, description, and preferred genre.
2. **Story Decomposition:** Gemini processes the narrative and generates structured cinematic scenes.
3. **Prompt Engineering:** Scene descriptions are converted into detailed prompts suitable for image generation.
4. **Character Integration:** Custom-trained LoRA weights can be integrated into the Stable Diffusion pipeline.
5. **Image Generation:** Stable Diffusion generates visual representations of individual scenes.
6. **Image Enhancement:** Optional face restoration and image refinement are applied.
7. **Storyboard Generation:** Generated frames are displayed through the Streamlit interface and made available for download.

## Installation and Execution

### Prerequisites

- Google Colab account.
- GPU-enabled runtime.
- Google Gemini API key.
- Ngrok authentication token.
- Internet connectivity.

### Execution Steps

1. Clone or download the repository.
2. Upload the Jupyter Notebook to Google Colab.
3. Enable GPU acceleration in the runtime settings.
4. Configure the required API credentials.
5. Execute the notebook cells sequentially.
6. Allow the environment to install dependencies and initialize the models.
7. Access the Streamlit application through the generated public URL.

## Character Training Workflow

1. Navigate to the character training section.
2. Upload reference images of the character.
3. Configure the character trigger token.
4. Set the training parameters.
5. Execute the LoRA training process.
6. Export the trained model weights.
7. Integrate the trained model into the storyboard generation workflow.

## Storyboard Generation Workflow

1. Navigate to the storyboard generation interface.
2. Enter the story title and description.
3. Select the preferred genre.
4. Configure the number of scenes.
5. Enable custom character LoRA integration if required.
6. Configure image resolution and generation settings.
7. Execute storyboard generation.
8. Preview and download the generated scene images.

## Project Structure

```text
FrameForge/
│
├── storyboard_final.ipynb
│
├── models/
├── training_images/
├── train_data/
├── output/
├── logs/
└── generated/
    ├── scene_1.png
    ├── scene_2.png
    └── scene_3.png
```

*Note: Runtime directories are illustrative and may be created dynamically during notebook execution.*

## Future Enhancements

- AI-powered storyboard-to-video generation.
- Text-to-video model integration.
- Multi-character consistency across scenes.
- Advanced reference-guided image generation.
- Automated storyboard PDF export.
- Video interpolation and scene transitions.
- Cloud-based model deployment.
- Interactive storyboard editing and regeneration.

## Project Objective

FrameForge aims to streamline the visual pre-production process by combining Large Language Models, diffusion-based image generation, and parameter-efficient model fine-tuning.

The platform demonstrates the practical integration of Generative AI technologies to automate narrative decomposition, cinematic prompt engineering, character customization, and visual content generation.

## Author

**Venkata Raja B Y**

AI/ML Developer | Generative AI | Full-Stack Development

GitHub: https://github.com/venkat2k25

---

