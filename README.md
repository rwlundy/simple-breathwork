# simple-breathwork

A simple, self-contained breathwork metronome — works eyes open or closed.

## Features

### Breathing Patterns
Several built-in patterns are included (Box Breathing, 4-7-8, etc.). You can also create your own using the **Build Pattern** link below the pattern selector.

### Custom Pattern Builder
The pattern builder lets you construct a sequence of Inhale, Hold, and Exhale steps with custom durations. Each step can be reordered by dragging or removed with the delete button. You can set the pattern to loop indefinitely or run a fixed number of repeats. When you save a pattern, it's given a name and appears alongside the built-in patterns.

**Storage:** Custom patterns are saved to `localStorage` under the key `breathwork_custom_patterns`. They persist across page refreshes and browser sessions on the same device, but are local to that browser — they won't sync across devices. Saved patterns can be deleted from the pattern selector by clicking the × next to them.

### Audio Options
Choose how each breath phase transition is signaled:

- **Tone** — a soft sine wave beep (default)
- **Wood Block** — a synthesized percussive click via Web Audio API
- **Gentle Voice** — speaks the phase name at each transition, then counts down each second using the Web Speech API
- **Mute** — no audio

### Background Images
Three rock garden images are available as backgrounds. Images are embedded as base64 directly in the HTML so the file remains fully self-contained and shareable without any external assets. A plain (no background) option is also available.

## Usage

Open `breathwork.html` in any modern browser — no server, build step, or internet connection required. Everything is in a single file.
