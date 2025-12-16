# Exercise Library - AI Generated Visual Assets

> **Built upon:** [wrkout/exercises.json](https://github.com/wrkout/exercises.json)
> This project contributes AI-generated video assets that complement the database's images and exercise descriptions. The quality of the generated videos varies, which can be attributed to the complexity of the exercise, and/or the quality of the description and the starting image that was used. 

## Overview

This repository provides **AI-generated exercise video demonstrations** for **873 exercises**.
**Many** exercises have issues, given that the generation is solely based on a starting image, combined with a prompt that includes the exercise to perform. 

### What's Included

- **📸 Position Images**: 2 images per exercise from the original db (Position 1 used for img2video generation, Position 2 for reference)
- **🎬 Videos**: MP4 videos demonstrating full movements (generated from Position 1 using img2video)
- **🎞️ Animated GIFs**: Optimized animations for web use
- **📝 Complete Metadata**: Instructions, muscles worked, equipment (from original db) + the AI generation prompts

**The image assets from the original repo had copyright limitations**, which has implications for the generated videos as well. Next steps will be to use style transfer, or use video generation without a starting image to disconnect from the copyrighted appearance. 

---

## Quick Start

### Browse Exercises

📖 **[View All 873 Exercises](EXERCISES.md)** - Complete visual catalog organized by category

### Example Exercise

Here's an example of what each exercise entry includes:

## Back Flyes - With Bands

| Attribute | Value |
|-----------|-------|
| **Category** | Strength |
| **Level** | Beginner |
| **Primary Muscles** | shoulders |
| **Secondary Muscles** | middle back, triceps |
| **Equipment** | Bands |
| **Force** | Pull |
| **Mechanic** | Compound |

### Instructions

1. Run a band around a stationary post like that of a squat rack.
2. Grab the band by the handles and stand back so that the tension in the band rises.
3. Extend and lift the arms straight in front of you. Tip: Your arms should be straight and parallel to the floor while perpendicular to your torso. Your feet should be firmly planted on the floor spread at shoulder width. This will be your starting position.
4. As you exhale, move your arms to the sides and back. Keep your arms extended and parallel to the floor. Continue the movement until the arms are extended to your sides.
5. After a pause, go back to the original position as you inhale.
6. Repeat for the recommended amount of repetitions.

### Demonstration

<table>
<tr>
<td align="center"><img src="exercises/Back_Flyes_-_With_Bands/images/0.jpg" alt="Position 1" width="300"/><br/><b>Position 1<br/>(used for img2video)</b></td>
<td align="center"><img src="exercises/Back_Flyes_-_With_Bands/gifs/0_quarter.gif" alt="Generated Video" width="300"/><br/><b>Generated Video</b></td>
<td align="center"><img src="exercises/Back_Flyes_-_With_Bands/images/1.jpg" alt="Position 2" width="300"/><br/><b>Position 2<br/>(not used for generation)</b></td>
</tr>
</table>

---

### Prompt for video generation

This is a Back Flyes - With Bands for strength that uses pull force to primarily train the shoulders. These are the instructions that a person would receive: \"Run a band around a stationary post like that of a squat rack. Grab the band by the handles and stand back so that the tension in the band rises. Extend and lift the arms straight in front of you. Tip: Your arms should be straight and parallel to the floor while perpendicular to your torso. Your feet should be firmly planted on the floor spread at shoulder width. This will be your starting position. As you exhale, move your arms to the sides and back. Keep your arms extended and parallel to the floor. Continue the movement until the arms are extended to your sides. After a pause, go back to the original position as you inhale. Repeat for the recommended amount of repetitions.

[**→ See all 873 exercises in EXERCISES.md**](EXERCISES.md)

---

## Statistics

- **Total Exercises**: 873
- **Categories**: 7
- **Total Images**: 1746
- **Total Videos**: 873
- **Total GIFs**: 873

**Categories**: Cardio, Olympic weightlifting, Plyometrics, Powerlifting, Strength, Stretching, Strongman

---

## About This Project

### Motivation

From [wrkout/exercises.json](https://github.com/wrkout/exercises.json) contributing guidelines:

> *"Exercise Images - NB: Any help in creating digital copyright free images for each exercise would be extremely helpful. Currently all exercises have two images, these have been scrapped off the internet, therefore l do not own the copy right for these images and would advise against using them in commercial projects."*
>
> *"Exercise Videos - Currently none of the exercises have videos, but if anyone can help in creating digital videos (or gifs) of each exercise, that again would be extremely helpful."*

### Process

All visual assets were generated using:
- **Platform**: Python script interfacing with ComfyUI pipelines
- **Model**: [Wan2.2 Image-to-Video 14B](https://github.com/Wan-Video/Wan2.2)
- **Source**: Videos/GIFs generated from Position 1 images based on exercise descriptions

Generation prompts are included in each exercise's `exercise_prompt.json` file for transparency.

---

## File Structure

```
exercises/
└── EXERCISE_NAME/
    ├── exercise.json              # Exercise metadata
    ├── exercise_prompt.json       # Exercise data with AI generation prompt
    ├── images/
    │   ├── 0.jpg                 # Position 1 (used for img2video)
    │   └── 1.jpg                 # Position 2 (reference only)
    ├── gifs/
    │   └── 0_quarter.gif         # Optimized animation (25% resolution)
    └── video/
        └── 0.mp4                 # Video demonstration
```


### Integration

All exercise data is in JSON format, making it easy to integrate into:
- Fitness tracking apps
- Workout builders
- Exercise databases
- Training platforms

---

## Credits & License

- **Original Database**: [wrkout/exercises.json](https://github.com/wrkout/exercises.json) by [@wrkout](https://github.com/wrkout)
- **AI Visual Assets**: Generated using ComfyUI and WAN 2.2 model
- **License**: Restricted, since the videos potentially inherit restrictions from the original images, which the original repo did not own. 

---

## Links

- 📖 [Browse All Exercises](EXERCISES.md)
- 🌐 [Web Viewer](index.html)
- 🔗 [Original Database](https://github.com/wrkout/exercises.json)
- 💬 [Report Issues](https://github.com/YOUR_USERNAME/YOUR_REPO_NAME/issues)

---
