# Physics-simulation-of-Fluid-dynamics-using-WALRUS
This project uses **WALRUS**, a physics foundation model, to predict how a heated fluid evolves over time using the **Rayleigh–Bénard convection** dataset.

Fluid Simulation Output:

<p align="center">
  <img src="https://raw.githubusercontent.com/debabratapruseth/Physics-simulation-of-Fluid-dynamics-using-WALRUS/main/Fluid%20Dynamics%20with%20Walrus.gif" width="150" height="300">
</p>

---
## Project Objective
The goal is to show how an AI model can look at the current state of a physical system and predict what happens next.
In simple terms:
> We show the AI a snapshot of heated fluid.  
> The AI predicts how the fluid will move and mix over time.
---
## Problem Statement
Physical systems such as fluids, weather, heat flow, and gases change over time.
Traditionally, these systems are simulated using numerical physics solvers. In this project, we use a machine learning model called **WALRUS** to forecast the future state of the system.

⸻

## Dataset Used

Dataset: Rayleigh–Bénard convection

This dataset represents a heated fluid system.

In this system:

* hot fluid rises
* cooler fluid sinks
* swirling patterns form
* the fluid gradually mixes over time

A simple analogy:

Imagine watching soup being heated in a pot.
Hot liquid rises, cooler liquid sinks, and patterns begin to form.

⸻

## Model Used

This project uses:

* WALRUS by PolymathicAI
* pretrained WALRUS checkpoint
* The Well-style physics dataset format

WALRUS predicts future states of physical systems across different scientific domains.

⸻

## Input and Output

Input

The input is a physics snapshot from the Rayleigh–Bénard dataset.

It is not a normal image. Each grid location stores scientific values such as fluid-related physical fields.

Conceptually:

Input = current state of fluid

Output

The output is a sequence of predicted future frames.

Output = predicted future fluid movement

The final visualization is a GIF:

Frame 1 → Frame 2 → Frame 3 → ... → Future fluid evolution

⸻

Final Output

The project generates a GIF of the fluid mixture prediction over time.

Color interpretation:

* dark / purple = lower value
* orange / red = medium value
* yellow / white = higher value

If the selected field represents temperature, brighter regions can be interpreted as hotter regions.

⸻

## Project Workflow

1. Set up Colab environment
2. Install WALRUS and dependencies
3. Download WALRUS pretrained checkpoint
4. Download Rayleigh–Bénard sample data
5. Load one physics batch
6. Run WALRUS autoregressive rollout
7. Generate predicted future frames
8. Convert predictions into colored heatmap frames
9. Save frames as a GIF

⸻

Layman Explanation

This project is like asking an AI to continue a physics movie.

We give it the current frame of a heated fluid system.
The AI predicts the next few frames.
Then we convert those predictions into a colored animation.

In simple words:

The model watches how the fluid looks now and imagines how it will mix in the future.

⸻

Portfolio Summary

This project demonstrates:

* physics-informed machine learning
* foundation model inference
* autoregressive prediction
* scientific visualization
* GIF generation from model outputs
* beginner-friendly explanation of complex simulation data

⸻


## Credits

* WALRUS: PolymathicAI
* Dataset: Rayleigh–Bénard convection from The Well
* Visualization: Matplotlib and ImageIO

⸻


## Related Blog and Research PDF

### This repository supports the blog post:

From Simulation to Prediction: Learning Fluid Dynamics with AI

https://debabratapruseth.com/from-simulation-to-prediction-learning-fluid-dynamics-with-ai/

### Research-style title:

Research PDF: https://debabratapruseth.com/wp-content/uploads/From-Simulation-to-Prediction-Data-Driven-Modeling-of-Fluid-Dynamics-Using-Artificial-Intelligence.pdf

### If you reference this project, please cite:

Pruseth, D. (2026). From Simulation to Prediction: Data-Driven Modeling of Fluid Dynamics Using Artificial Intelligence.

⸻

## License

This project is licensed under the MIT License — you’re free to use, modify, and distribute it.

