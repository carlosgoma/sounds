# 🎧 Sample Library

This repository contains a personal sound library.

---

## 🧱 Naming Convention

General format:
Not all fields are required.

```
[type]_[category]_[descriptor]_[extra].wav

```

---

## 🧩 1. Type (usage / duration)

Defines how the sound is typically used:

* `loop` → rhythmic or syncable loops
* `shot` → short one-shots
* `tex` → textures / ambient / non-rhythmic sounds
* `vox` → vocals

---

## 🧩 2. Category (sound family)

* `drum` → standard drum elements (kick, snare, hi-hat, drum loops)
* `bass` → low-frequency tonal elements (basslines, sub, low drones)
* `mel` → melodic or harmonic elements (leads, chords, arpeggios)
* `fx` → sound effects and transitions (impacts, risers, glitches, sweeps)
* `amb` → ambient or environmental textures (drones, atmospheres, field recordings)
* `perc` → non-standard percussive elements (clicks, taps, metallic or organic hits)

---

## 🧩 3. Descriptor (character)

Free but controlled vocabulary describing the sound:

Examples:

* `dark`, `soft`, `noisy`, `glitch`, `industrial`, `organic`
* `kick`, `snare`, `hat`, `clap` (for drums)

---

## 🧩 4. Extra metadata (optional)

Used only when relevant:

* Key → `C`, `Am`, `F#`
* BPM → `120`, `140`
* Length (musical) → `4bar`, `8bar`
* Size class → `S`, `M`, `L`
* Version → `v1`, `v2`

---

## 🔥 Examples


```
tex_amb_drone_dark.wav
tex_amb_wind_soft.wav
tex_amb_glitch_noise.wav
tex_amb_drone_L.wav
loop_amb_pulse_soft_100bpm_4bar.wav
loop_amb_pulse_120bpm_8bar.wav
loop_bass_groove_A_120.wav
shot_drum_kick_punchy.wav
shot_perc_click_glitch.wav
vox_phrase_female_C_120.wav
vox_texture_whisper_dark.wav
```

---

## ⚠️ Guidelines

* Keep naming consistent
* Use snakecase, only camelcase on the descriptor
* Add metadata only when useful

---

## 🚀 Usage Tip

Filter:

```js
samples.filter(s => s.includes("kick"))
samples.filter(s => s.startsWith("loop_"))
samples.filter(s => /_120bpm/.test(s))
```

