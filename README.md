# Audio-Visualizer
# Ultimate Audio Visualizer Pro

## ⚠️ CRITICAL HEALTH WARNING ⚠️

**🚨 SEIZURE AND PHOTOSENSITIVE EPILEPSY WARNING 🚨**

**THIS APPLICATION CONTAINS RAPIDLY FLASHING LIGHTS, STROBING EFFECTS, AND INTENSE VISUAL PATTERNS THAT MAY TRIGGER SEIZURES IN INDIVIDUALS WITH PHOTOSENSITIVE EPILEPSY OR OTHER LIGHT-SENSITIVE CONDITIONS**

### DO NOT USE THIS APPLICATION IF YOU:
- Have a history of seizures or epilepsy
- Have photosensitive epilepsy or light-triggered seizures
- Are sensitive to flashing lights or rapid visual changes
- Experience migraines, headaches, or dizziness from visual stimuli
- Have any neurological conditions that may be affected by intense visual effects

### VISUAL EFFECTS INCLUDE:
- Rapid flashing and strobing lights at frequencies up to 60Hz
- Intense color cycling and sudden color changes
- High-contrast patterns and geometric distortions
- Beat-synchronized light flashes and explosions
- Pulsing, rotating, and morphing visual elements
- Kaleidoscopic and fractal patterns

**BY USING THIS SOFTWARE, YOU ACKNOWLEDGE THAT YOU HAVE READ THIS WARNING AND UNDERSTAND THE RISKS. USE AT YOUR OWN RISK.**

---

## Overview

A real-time WebGL audio visualizer that creates stunning visual effects synchronized to microphone input or system audio. Features multiple visualization modes, extensive customization options, and advanced shader-based graphics.

## Features

### Visualization Modes
- **🌀 Fractal Reactor** - Multi-layered 3D fractals with orbital motion
- **🕳️ 3D Tunnel** - Endless tunnel with beat-reactive deformation and particle bursts
- **🌈 Psychedelic Fractal** - Fullscreen shader-based kaleidoscopic fractals
- **🔮 DMT Tunnel** - Immersive shader tunnel with complex pattern generation

### Audio Analysis
- Real-time FFT analysis with 4096 sample buffer
- Frequency band separation (bass, mid, treble)
- Advanced beat detection with energy threshold analysis
- RMS energy calculation and trend analysis
- 32-band spectrum analyzer with smoothing

### Visual Effects
- **Beat-Reactive Elements** - Explosions, flashes, and scaling on beat detection
- **Particle Burst Systems** - Dynamic particle generation on audio peaks
- **Color Theme Engine** - 8 predefined themes with real-time switching
- **Dynamic Camera Effects** - Camera movement and shake based on audio
- **Performance Scaling** - Automatic quality adjustment based on device capabilities

### Advanced Controls
- **Sensitivity** - Audio input responsiveness (0.1-5.0)
- **Speed** - Animation and movement rate (0.1-4.0)
- **Intensity** - Overall visual energy and brightness (0.1-5.0)
- **Zoom** - Visual scale and perspective (0.1-5.0)
- **Contrast** - Light/dark ratio and opacity (0.1-3.0)
- **Orbit Size** - Particle and element movement radius (0.1-3.0)
- **Color Shift** - Color cycling speed (0.1-5.0)
- **Center X** - Horizontal visual offset (-2.0 to 2.0)
- **Symmetry** - Kaleidoscope mirror count (3-20)
- **Rotation** - Spinning element speed (0.1-5.0)
- **Warp** - Distortion and deformation amount (0.0-2.0)
- **Iterations** - Fractal detail level (20-200)
- **Flow Speed** - Shader animation rate (0.1-3.0)
- **Complexity** - Pattern intricacy (0.5-3.0)
- **Distortion** - Global visual warping (0.0-2.0)
- **Kaleidoscope** - Mirror effect strength (0.0-3.0)
- **Morphing** - Shape transformation rate (0.0-2.0)
- **Fractal Depth** - Recursive pattern depth (0.5-3.0)

## Usage

### Getting Started
1. Open the HTML file in a modern web browser (Chrome, Firefox, Safari, Edge)
2. Click "🎤 Start Microphone" to begin audio capture
3. Grant microphone permissions when prompted
4. Play music or make sounds to see the visualizations react

### Controls
- **Space Bar** - Start/stop audio capture
- **F11** - Toggle fullscreen mode
- **H** - Hide/show control panel
- **1-4 Keys** - Quick switch between visualization modes
- **Mouse** - Adjust sliders and dropdown menus in real-time

### Color Themes
- **Cyan Glow** - Classic cyan and blue tones
- **Rainbow** - Multi-color spectrum cycling
- **Fire** - Orange, red, and yellow flames
- **Electric Blue** - Various blue electric tones
- **Neon Pink** - Bright pink and magenta
- **Matrix Green** - Classic green matrix effects
- **Sunset** - Warm orange and yellow gradients
- **Cosmic Purple** - Deep space purple and blue

### Background Modes
- **Gradient** - Animated color gradients
- **Dark** - Pure black background
- **Stars** - Twinkling starfield effect
- **Matrix** - Animated matrix rain pattern
- **Cosmic** - Nebula and space effects

## Technical Requirements

### Browser Support
- Chrome 60+ (recommended)
- Firefox 55+
- Safari 11+
- Edge 79+

### Hardware Requirements
- WebGL-capable graphics card
- Microphone access for audio input
- Minimum 4GB RAM recommended
- Dedicated GPU recommended for High quality mode

### Performance Levels
- **High** - Full effects, 60+ FPS, high particle counts
- **Medium** - Reduced particle counts, medium quality shaders
- **Low** - Minimal effects for older hardware

## Installation

### Local Usage
1. Download the `audio-visualizer.html` file
2. Open directly in a web browser
3. No additional dependencies required

### Web Hosting
1. Upload the HTML file to any web server
2. Ensure HTTPS for microphone access
3. No build process or compilation needed

## Customization

### Modifying Color Themes
Edit the `colorThemes` object in the JavaScript code:

```javascript
this.colorThemes = {
    custom: { 
        primary: 0xff0000,    // Red
        secondary: 0x00ff00,  // Green  
        accent: 0x0000ff      // Blue
    }
};
```

### Adding New Modes
1. Create a new visualizer class extending the base pattern
2. Add mode to `modeControls` and `modeDefaults` objects
3. Include in the switch statement in `switchVisualizer()`

### Performance Tuning
Adjust these variables for different hardware:
- `segmentCount` - Number of tunnel segments
- `particleCount` - Total particles rendered
- `fftSize` - Audio analysis resolution (1024-8192)

## Troubleshooting

### Common Issues
- **Black Screen** - Check WebGL support in browser
- **No Audio Response** - Verify microphone permissions
- **Poor Performance** - Lower quality settings or close other applications
- **Distorted Visuals** - Reset controls to default values

### Browser Permissions
- Microphone access required for audio input
- Fullscreen API access for immersive experience
- Hardware acceleration should be enabled

## Safety Guidelines

### Recommended Usage
- Take breaks every 15-30 minutes during extended use
- Use in well-lit rooms to reduce eye strain
- Start with lower intensity settings and gradually increase
- Ensure comfortable viewing distance from the screen
- Stop immediately if experiencing any discomfort

### Signs to Stop Using Immediately
- Dizziness or nausea
- Headaches or eye strain
- Any unusual visual sensations
- Feeling disoriented or confused
- Any physical discomfort

## Legal Disclaimer

**This software is provided "AS IS" without warranty of any kind. The authors and contributors are not responsible for any adverse health effects, seizures, or other medical conditions that may result from the use of this software. Users assume all risks associated with its use.**

**If you have any medical conditions or concerns about photosensitive reactions, consult with a healthcare professional before using this application.**

## Technical Architecture

### Core Components
- **Three.js (r128)** - 3D graphics rendering engine
- **Web Audio API** - Real-time audio analysis
- **WebGL Shaders** - GPU-accelerated visual effects
- **Responsive Design** - Mobile and desktop compatibility

### Audio Processing Pipeline
1. Microphone input capture via getUserMedia()
2. Web Audio API analysis with configurable FFT size
3. Frequency band separation and RMS calculation
4. Beat detection using energy threshold analysis
5. Real-time visual parameter mapping

### Rendering Pipeline
1. Dynamic performance level detection
2. GPU capability assessment and optimization
3. Adaptive quality scaling based on framerate
4. Multi-threaded shader compilation
5. 60fps target with graceful degradation

## Contributing

### Development Setup
1. Clone the repository
2. Open the HTML file in a browser with a live reload extension
3. Edit JavaScript directly in the file
4. Test across different browsers and devices

### Code Structure
- Main visualizer class handles initialization and coordination
- Individual visualizer classes for each mode
- Modular audio analysis system
- Shader programs for GPU-accelerated effects

## License

This project is open source. Please ensure you comply with Three.js licensing terms and include appropriate health warnings when redistributing.

---

**Remember: Always prioritize your health and safety when using visual effects software. If in doubt, don't use it.**
