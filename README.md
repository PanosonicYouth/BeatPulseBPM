# Beat Pulse (BPM)

Current Version: v0.1.3 (beta)

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

## Prerequisites (important)

- You need the **exact BPM** of your track.  
  **Recommended:** use a DAW (e.g. **Ableton Live**) to *identify/confirm* the BPM and (ideally) **warp/enforce a constant tempo** before animating.

- For best results, your audio should start **exactly on Beat 1** (no gap/silence before the first downbeat).  
  If your track starts late, you can either:
  - **trim/slide the audio** so the first downbeat lands at the start of the timeline, **or**
  - compensate using **Phase → Custom (beats)** and keyframe **Custom Phase (beats)** to align.

---

## Download

1. Go to the latest Release:  
   https://github.com/PanosonicYouth/BeatPulseBPM/releases/latest
2. Under **Assets**, download:  
   - ✅ **BeatPulseBPM_VX.X.X.zip** *(recommended — includes the `.fuse`, PDF manual, and demo project)*  
   - or download individual files: `BeatPulseBPM.fuse`, `BeatPulseBPM_Manual.pdf`, `BeatPulseDemo.zip`
  
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
