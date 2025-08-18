# Simple CSS Animations

A lightweight collection of simple, performant CSS animations for modern web applications. This library provides a comprehensive set of keyframe animations using modern CSS properties like `translate`, `scale`, and `rotate` for optimal performance.

## Installation

```bash
npm install @danilidonbeltran/simple-css-animations
```

## Usage

### Import the entire library
```css
@import url("@danilidonbeltran/simple-css-animations");
```

### Import specific animation types
```css
@import url("@danilidonbeltran/simple-css-animations/src/show-animations.css");
@import url("@danilidonbeltran/simple-css-animations/src/hide-animations.css");
```

### Apply animations to elements
```css
.animated-element {
  animation: bounce-in 1s ease-out;
}

.fade-element {
  animation: fade-in 0.5s ease-in-out;
}
```

## Available Animations

### Show/Entrance Animations

#### Bounce Animations
- `bounce` - Simple bouncing effect
- `bounce-in` - Bouncing entrance with scale
- `bounce-in-left` - Bounce in from the left
- `bounce-in-right` - Bounce in from the right
- `bounce-in-up` - Bounce in from above
- `bounce-in-down` - Bounce in from below

#### Fade Animations
- `fade-in` - Simple fade in
- `fade-in-up` - Fade in while moving up
- `fade-in-down` - Fade in while moving down
- `fade-in-left` - Fade in while moving from left
- `fade-in-right` - Fade in while moving from right

#### Slide Animations
- `slide-in` - Generic slide in
- `slide-in-right` - Slide in from the right
- `slide-in-left` - Slide in from the left
- `slide-in-top` - Slide in from the top
- `slide-in-bottom` - Slide in from the bottom

#### Zoom Animations
- `zoom-in` - Simple zoom in
- `zoom-in-down` - Zoom in from above
- `zoom-in-up` - Zoom in from below
- `zoom-in-left` - Zoom in from the left
- `zoom-in-right` - Zoom in from the right

#### Roll Animations
- `roll-in-right` - Roll in from the right
- `roll-in-left` - Roll in from the left

#### Rotation Animations
- `rotate` - Simple rotation
- `rotate-in` - Rotating entrance

#### Special Effects
- `flash` - Flashing effect
- `flip` - Simple flip
- `flip-in` - Flipping entrance
- `heartbeat` - Heartbeat pulse effect
- `jack-in-the-box` - Spring-like entrance
- `light-speed-in` - High-speed entrance
- `pulse` - Pulsing effect
- `shake` - Shaking effect
- `swing` - Swinging motion
- `tada` - Celebration effect
- `wobble` - Wobbling motion

### Hide/Exit Animations

#### Bounce Out Animations
- `bounce-out` - Bouncing exit with scale
- `bounce-out-left` - Bounce out to the left
- `bounce-out-right` - Bounce out to the right
- `bounce-out-up` - Bounce out upward
- `bounce-out-down` - Bounce out downward

#### Fade Out Animations
- `fade-out` - Simple fade out
- `fade-out-up` - Fade out while moving up
- `fade-out-down` - Fade out while moving down
- `fade-out-left` - Fade out while moving left
- `fade-out-right` - Fade out while moving right

#### Slide Out Animations
- `slide-out` - Generic slide out
- `slide-out-right` - Slide out to the right
- `slide-out-left` - Slide out to the left
- `slide-out-top` - Slide out to the top
- `slide-out-bottom` - Slide out to the bottom

#### Zoom Out Animations
- `zoom-out` - Simple zoom out
- `zoom-out-down` - Zoom out downward
- `zoom-out-up` - Zoom out upward
- `zoom-out-left` - Zoom out to the left
- `zoom-out-right` - Zoom out to the right

#### Roll Out Animations
- `roll-out-right` - Roll out to the right
- `roll-out-left` - Roll out to the left

#### Other Exit Effects
- `flip-out` - Flipping exit
- `light-speed-out` - High-speed exit
- `rotate-out` - Rotating exit

## Examples

### Basic Usage
```html
<div class="box" style="animation: bounce-in 1s ease-out;">
  Hello World!
</div>
```

### Chaining Animations
```css
.element {
  animation: fade-in 0.5s ease-in-out;
}

.element.exit {
  animation: fade-out 0.3s ease-in-out;
}
```

### Custom Timing
```css
.slow-bounce {
  animation: bounce-in 2s ease-out;
}

.fast-fade {
  animation: fade-in 0.2s ease-in-out;
}
```

### Animation with Delays
```css
.delayed-animation {
  animation: slide-in-right 0.6s ease-out 0.3s both;
}
```

## Browser Support

These animations use modern CSS properties and are optimized for performance:
- Uses `translate`, `scale`, and `rotate` for hardware acceleration
- Compatible with all modern browsers
- Optimized for 60fps animations

## Performance Notes

- All animations use transform properties (`translate`, `scale`, `rotate`) which are GPU-accelerated
- Avoid animating layout-affecting properties for best performance
- Consider using `animation-fill-mode: both` to maintain start/end states

## License

ISC License - see package.json for details.

## Author

Daniel J.L. Beltran

## Repository

[GitHub Repository](https://github.com/dani-beltran/simple-css-animations)