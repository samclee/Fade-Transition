# Fade Transition
## Description
[Download it here](https://godotengine.org/asset-library/asset/1663)

A node for covering and uncovering the screen with a fading effect. Created for Godot 4.

## Properties
|Type | Name | Default value|
|---|---|---|
|float | default_cover_duration | 0.3 |
|float | default_uncover_duration | 0.2 |
|bool | initially_covering | false |
|TransitionType | cover_transition | TRANS_EXPO |
|EaseType | cover_ease | EASE_OUT |
|TransitionType | uncover_transition | TRANS_EXPO |
|EaseType | uncover_ease | EASE_OUT |

## Methods
Return type | Signature
---|---
void | cover(float duration=default_cover_duration)
void | uncover(float duration=default_uncover_duration)
void | set_covered()
bool | is_running() const

## Signals



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
