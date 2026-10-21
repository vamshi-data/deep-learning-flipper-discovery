# Deep Learning Flipper Discovery

A browser-based interactive teaching tool that uses a pinball-inspired analogy to explain how deep learning models learn from input data, update weights, and make predictions.

This project turns abstract ideas like pixels, weights, layers, and error correction into a visual system that can be explored directly in the browser.

## What this project shows

- An 8x8 handwritten digit sample mapped into 64 input signals
- A layered “flipper network” that redirects moving balls through the system
- Learnable spring-dot weights that change as the model updates
- Layer-by-layer timing and freezing to illustrate how information flows through a deep model
- A simplified training loop showing prediction, error, and correction

## Why it exists

The visual model is intentionally an analogy, not a mathematically exact implementation of deep learning. It is designed to help learners connect:

- raw input values to network activations
- learned parameters to directional influence
- Hidden layers to representation building
- prediction error to weight updates
- repeated examples to learning over time

## Project structure

- `index.html` — the complete interactive experience and training simulation
- `README.md` — project overview and usage notes

## Run locally

Because this is a static HTML app, you can open it directly in a browser or serve it locally:

### Option 1: Open directly

Open `index.html` in your browser.

### Option 2: Serve locally

From the project directory:

```bash
python -m http.server 8000
```

Then open:

```text
http://localhost:8000
```

## Features

- Interactive pinball-style visualization
- Adjustable number of layers and flipper counts
- Per-layer freeze timers and motion controls
- Learning-rate and target-digit controls
- Weight diagnostics and training progress feedback
- A conceptual guide explaining the deep learning ideas behind the analogy

## Educational framing

The project is designed around the core learning loop:

1. See the input
2. Propagate through the network
3. Predict an output
4. Compare with the target
5. Correct the parameters
6. Repeat

This mirrors the way training works in real neural networks, while keeping the visual metaphors intuitive and approachable.

## Notes

- This is a teaching visualization, not a production deep learning framework.
- The pinball mechanics are used as a conceptual bridge to explain weight updates, layers, and credit assignment.
- The displayed sample data is based on the scikit-learn handwritten digits dataset.

## License

This project does not currently declare a specific license. If you plan to reuse or publish it, check whether a license is intended before distributing the code.

## Credits

The project is built as an educational interactive simulation and references the scikit-learn digits dataset for its handwritten-digit examples.
