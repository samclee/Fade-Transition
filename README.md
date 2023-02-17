# Fade Transition
A node for covering and uncovering the screen with a fading effect.

## Usage
### Covering the screen
1. Instantiate a `FadeTransition` node in your scene
2. Call the `cover()` function on the `FadeTransition`

### Uncovering the screen
1. Instantiate a `FadeTransition` node in your scene
2. Call the `uncover()` function on the `FadeTransition`

### Signals
The `FadeTransition` node will emit `cover_done` and `uncover_done` signals when its `cover()` and `uncover()` methods are finished respectively.

## FAQ
### Why do you use terms like "cover" and "uncover"
I keep confusing myself when I think if "fading out" means the screen is fading out (to black) or the screen cover is fading out (to transparency).
