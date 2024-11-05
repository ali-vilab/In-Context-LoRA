# Getting Started

- [x] Training & Inference Code: Released (directly uses [AI-Toolkit](https://github.com/ostris/ai-toolkit))
- [x] Sample Training Data & Configuration File: Available in this repository for easy setup
- [ ] Model Checkpoints: Comming Soon

You can directly use the open-source [AI-Toolkit](https://github.com/ostris/ai-toolkit) to train IC-LoRA models. We have provided sample training data with a configuration file in this repo:

- **Configuration File**: `config/movie-shots.yml` (place it in the `config/` directory of AI-Toolkit)
- **Sample Training Data**: `data/movie-shots.zip` (extract it to `data/movie-shots` of AI-Toolkit)

After installing the necessary dependencies and setting up AI-Toolkit, you can start training by running:

```bash
python run.py config/movie-shots.yml
```

The training runs on a single GPU with at least 24GB of memory (adjust the `resolution` parameter in `config/movie-shots.yml` for different GPU memory limits). The training should complete in a few hours.

## Prompt for Multi-Scene Image Captioning

As a reference, we provide an example prompt used to generate captions for multi-scene images:

> *Create a short description of this three-scene image featuring movie shots, beginning with the prefix [MOVIE-SHOTS] for the entire caption, followed by an overall summary of the image. Each scene detail should flow within the same sentence, with specific markers [SCENE-1], [SCENE-2], [SCENE-3], indicating the start of each scene’s description. Name the role(s) with random name(s) if necessary, and wrap the name(s) with "<" and ">". Ensure the entire description is cohesive, flows as one sentence, and remains within 512 words.*

## MODEL ZOO

We will continue to release In-Context LoRA models. Please stay tuned.
