---
name: ig-hindi-voiceover
description: Generate an original Hindi voiceover for reels for free with local text-to-speech, matched in style (energy, pace, tone) to what works in the niche. Use when a reel script needs audio, or the user says "awaz banao", "voiceover", "audio banao".
---

# Hindi voiceover

## What is allowed
- An original TTS voice, the user's own recorded voice, or a clone of the user's own voice made with their consent.
- Matching the *style* of a reference (energetic, calm storyteller, fast-paced explainer).
- Music: Instagram's in-app audio library (added at upload time), or royalty-free tracks with the licence noted.

## What is not done
- Cloning or imitating another creator's or celebrity's voice.
- Extracting and reusing audio from someone else's reel.
If the user asks for these, explain briefly and offer the closest original voice instead.

## Free pipeline (edge-tts)
1. `pip install edge-tts` (once). Hindi voices: `hi-IN-MadhurNeural` (male), `hi-IN-SwaraNeural` (female).
2. Put the voiceover lines (Devanagari) from `script.md` into `vo.txt`, one scene per line.
3. Generate per scene so timing can be matched:
   `edge-tts --voice hi-IN-MadhurNeural --rate=+8% --pitch=+0Hz --text "<line>" --write-media scene-01.mp3 --write-subtitles scene-01.vtt`
4. Style tuning: energetic → rate +10-15%; storyteller → rate -5%, add pauses with commas/। ; keep English brand words in Roman so they are pronounced correctly.
5. Listen back / check durations with `ffprobe`; total must fit the script length. Fix mispronounced words by respelling phonetically.
6. Join with ffmpeg, normalise loudness (about -14 LUFS), save `content/<item>/voiceover.mp3` plus the `.vtt` files for captions.

For other local tools (music, SFX, mixing) follow the `media-use` skill.

## Output
Audio file path, duration per scene, voice used. Let the user hear it before the video is built.
