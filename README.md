# M4L MotionHub Controller

**v1.1.0**

A Max for Live device for controlling [MotionHub](https://github.com/jp206100/motion-hub) visuals via OSC from Ableton Live.

## Features

- **8 OSC Parameters** for real-time visual control
- **Audio Follower** with peak amplitude detection, adjustable window and slide times, and gating
- **LFO Section** for automated parameter modulation
- Sends OSC messages to `localhost:9000`

## Parameters

| Parameter | OSC Address | Description |
|-----------|-------------|-------------|
| Glitch | `/motionhub/glitch` | Glitch amount (0-1) |
| Color Shift | `/motionhub/colorshift` + `/motionhub/intensity` | Color shift & intensity (0-1) |
| Speed | `/motionhub/speed` | Animation speed (1-4x) |
| Freq Min | `/motionhub/freqmin` | Minimum frequency in Hz |
| Freq Max | `/motionhub/freqmax` | Maximum frequency in Hz |
| Pulse | `/motionhub/pulse` | Pulse effect amount (0-1) |
| Monochrome | `/motionhub/monochrome` | Toggle monochrome mode |
| Reset | `/motionhub/reset` | Reset visuals trigger |

## Installation

1. Download `UJ MH Connect.amxd`
2. Place it in your Ableton Live User Library:
   - **macOS**: `~/Music/Ableton/User Library/Presets/MIDI Effects/Max MIDI Effect/`
   - **Windows**: `\Users\[username]\Documents\Ableton\User Library\Presets\MIDI Effects\Max MIDI Effect\`
3. Or simply drag and drop it onto a MIDI track in Ableton Live

## Usage

1. Launch **MotionHub** and enable OSC (default port: 9000)
2. In Ableton Live, add the **UJ MH Connect** device to any MIDI track
3. Use the sliders to control visual parameters in real-time
4. Enable the **Audio Follower** to react to your music
5. Use the **LFO** for automated parameter modulation

## Requirements

- Ableton Live 10+ with Max for Live
- [MotionHub](https://github.com/jp206100/motion-hub) application

## License

MIT License
