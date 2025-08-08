How It Works

Ray-march shader	Combines a Mandelbrot field, a Julia slice, and a 1-D Cantor dust mask into a single signed pseudo-distance function, then colors the hit point with a cosine palette for smooth gradients.

Camera controls	Arrow keys yaw/pitch; Page Up/Down move the camera forward/back along its local Z; holding Shift multiplies speed ×5 for rapid dives.

Tween.js	Included so you can easily add animated fly-throughs—call new TWEEN.Tween(camera.position) anywhere to script paths.

Performance	The shader steps only 128 iterations and exits early on hit for ~60 FPS on desktop GPUs. Tune iteration counts for your device.

Swap the distance estimator map() with a true Mandelbulb or quaternion Julia for richer 3-D structure.

Use ToneMapping and post-processing (e.g., bloom) from Three.js’ EffectComposer to mimic the glowing aesthetic of the sample image.

Add Tween.js camera rails triggered by GUI buttons to create curated tours through the fractal cavern.

Enjoy exploring the infinite depth and variation that arises when classical fractals meet modern GPU ray marching in Three.js!
