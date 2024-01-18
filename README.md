# Lip Syncing

## Overview

This repository contains a system to generate lip-synced videos using the Wav2Lip model. The process involves generating English and Arabic audio using text-to-speech models and creating corresponding lip-synced videos with diffusion models.

## Steps

1. **Text-to-Speech (TTS) Audio Generation:**

   - English TTS: Utilizes gTTS (Google Text-to-Speech) to convert English text to audio.

   - Arabic TTS: Translates English text to Arabic using transformers and generates Arabic audio with gTTS.

2. **Image Generation:**

   - Uses the Diffusion Models to generate images from text.
     
3. **Wav2Lip Lip Sync Video Generation:**

   - Processes the generated image and audio with Wav2Lip to create a lip-synced video.
     - Example command: `python3.6 inference.py --checkpoint_path checkpoints/wav2lip_gan.pth --face generated_image.png --audio English_audio.wav --outfile lip_sync_video.mp4`

4. **Dependencies:**

   - gTTS, transformers, sentencepiece for TTS.
   - Diffusion Models for image generation.
   - Wav2Lip for lip-sync video generation.

6. **Acknowledgments:**

   - Wav2Lip model by [Wav2Lip Repo](https://github.com/Rudrabha/Wav2Lip).

7. **Conclusion:**

   - This repository provides an end-to-end solution for generating lip-synced videos with text-to-speech audio. Feel free to explore different inputs and experiment with the provided model.

## Note
The test samples are in data_samples directory and the results in results directory
