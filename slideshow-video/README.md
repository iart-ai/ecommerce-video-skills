# Slideshow Video

Turn a set of photos into a finished video that feels shot, not assembled. Each still gets its own gentle Ken Burns motion (deterministic per index, so no two slides move the same way), slides change on the music beat, mixed portrait/landscape shapes are handled without stretching, and the whole folder reads through one template so the same setup renders any set of images. Built for anyone turning a folder of product or event photos into a montage, recap, or memories video.

## When it activates

- "Make a photo slideshow" / "turn photos into a video" / "create a photo montage video".
- "Make a picture slideshow with music" or "build a memories/recap video from photos".
- "Add Ken Burns pan/zoom to photos" or "sync slide changes to the music beat".
- "Render a video from a folder of images".

## Example prompts

- "Turn this folder of trip photos into a slideshow with Ken Burns motion and a crossfade."
- "Make a memories recap from these photos, snap slide changes to the music beat."
- "Build a slideshow that handles my mixed portrait and landscape shots without cropping faces."

## What's inside

- `SKILL.md` — the one rule (seeded, never-identical motion), per-photo Ken Burns, single consistent transitions, beat/music-synced pacing, mixed aspect-ratio handling (blurred-pad/cover/fit), captions and intro/outro cards, and folder→video templating.
- `references/ken-burns.md` — the complete seeded `<KenBurnsImage>` component with subject-aware anchoring and an FFmpeg `zoompan` equivalent.
- `references/timing-and-audio.md` — beat detection with librosa, beat-seconds → frame conversion, musical-unit slide assignment, and a BPM-grid fallback.
- `references/aspect-and-layout.md` — orientation detection, the blurred-pad/cover/contain layouts, and safe zones for 16:9, 9:16 and 1:1.
- `references/templating-folder.md` — the folder→manifest builder, the data-driven `<Slideshow>` with intro/outro cards, and a pure-FFmpeg pipeline.

---
Part of **[E-Commerce Video Skills](../)** · Built by **[iart.ai](https://iart.ai)** — controllable Motion Graphics MP4 from a prompt or data.
