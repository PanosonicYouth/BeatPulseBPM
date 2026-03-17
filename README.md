# Beat Pulse (BPM)

Current Version: v0.1.1 (beta)

Beat Pulse (BPM) is a DaVinci Resolve **Fusion modifier** that beat-syncs **any numeric parameter** to music (Angle, Size/Zoom, Glow, Blur, Opacity, etc.).

Stack up to **4 pulses**, use **musical note divisions** (straight / triplet / dotted), and choose between **Envelope** and **Oscillator** modes for clean rhythmic motion without drawing keyframes.

---

## Features

- **4 pulse layers** (Pulse 1–4) you can stack
- **Timing modes**
  - **Manual (beats)** — type `1`, `0.5`, `0.3333`, `4`, etc.
  - **Musical (notes)** — bar/half/quarter/eighth/16th + straight/triplet/dotted
- **Generator modes**
  - **Pulse (Envelope)** — hits/pumps/gates
  - **Oscillator (Waveform)** — smooth LFO motion (sway/wobble)
- **Polarity**: Unipolar (0..1) / Bipolar (-1..1)
- **Final operation**: Add / Multiply / Replace

---

## Install

1. Download `BeatPulseModifier.fuse`
2. Copy it into your Fusion Fuses folder:

**Windows (system-wide)**
```text
C:\ProgramData\Blackmagic Design\DaVinci Resolve\Fusion\Fuses\
```

**Windows (per-user)**
```text
C:\Users\<YOU>\AppData\Roaming\Blackmagic Design\DaVinci Resolve\Support\Fusion\Fuses\
```

**macOS (per-user)**
```text
~/Library/Application Support/Blackmagic Design/DaVinci Resolve/Support/Fusion/Fuses/
```

3. Restart DaVinci Resolve

---

## Usage (Quick Start)

1. Go to the **Fusion** page.
2. Right-click a numeric control (e.g. Transform → Angle/Size) → **Modify With → Modifiers → Beat Pulse (BPM)**.
3. In **Inspector → Modifiers**, set Master:
   - **BPM**
   - **FPS Preset** (match your timeline)
   - **Beats per Bar** (optional, default 4)
4. Enable **Pulse 1** and set:
   - **Pulse Timing** → Musical (notes)
   - **Note Division** → Quarter
   - **Feel** → Straight
   - Adjust **Amount**

**Tip:** Open the **Spline** editor and zoom in to view the waveform clearly.

---

## Documentation

- PDF Manual: `docs/BeatPulseBPM_Manual.pdf`

---

## License (Summary)

This project is **source-available** under the custom license in `LICENSE`.

- ✅ Free to use (including commercially) and modify for personal/internal use
- ✅ You may share the **unmodified** original release for free with attribution
- ❌ No selling, bundling, or redistributing modified versions
- ✅ Improvements can be submitted via pull requests

---

## Support / Feedback

Open an Issue and include:
- Resolve version + OS
- steps to reproduce
- screenshots / short screen recording if possible
