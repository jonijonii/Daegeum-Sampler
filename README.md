# Daegeum (Korean Traditional Wind Instrument) - Decent Sampler Library
This is a Decent Sampler virtual instrument library featuring the Daegeum (Sanjo), a representative traditional Korean bamboo flute. It captures the instrument's deep resonance and unique vibrato (Nonghyeon).

🎵 Introduction
This project processes a single raw recording source (sanjo_deageum_scale_vib_39.wav) into a playable virtual instrument using a custom Python pipeline.

Unlike standard auto-slicing methods which often mistake the Daegeum's breathy texture and vibrato for silence, this library uses an Envelope Smoothing Algorithm to perfectly preserve the authentic "Nonghyeon" (Korean traditional vibrato) without chopping the sound.

✨ Features
Authentic Tone: Captures the deep, buzzing timbre produced by the Cheong (membrane) of the Daegeum.

Vibrato (Nonghyeon) Preservation: No artificial tuning was applied. The performer's natural pitch fluctuations and ornaments (Sigimsae) are kept intact for realism.

18 Key Samples: Contains 18 distinct samples ranging from C4 to F#6. These samples are mapped using a nearest-neighbor algorithm to cover the full playable range with minimal pitch shifting.

Zero Delay Attack: Leading silence has been precisely trimmed to ensure immediate response for fast playing techniques (e.g., 16th notes).

Retina UI Support: High-resolution custom UI generated programmatically using Pillow (PIL), optimized for iPad and desktop screens.

🛠 Tech Stack
Python 3.x
Librosa: Audio signal processing & precision trimming.
Pandas & NumPy: Waveform envelope analysis.
Pillow (PIL): High-resolution UI generation & text rendering.

🚀 Installation (How to use)
To use this library in Decent Sampler, follow these steps to create a .dslibrary file:

Download Files: Download the following three items from this repository:

📂 Folder: Daegeum_Final_Samples

📄 File: Daegeum_Sanjo_Final.dspreset

🖼️ Image: Skin_Daegeum_Retina.jpg

Zip: Select these three items and compress them into a single ZIP file.

Rename: Change the file extension from .zip to .dslibrary.

Example: Archive.zip -> Daegeum_Sanjo.dslibrary

Import: Open the Decent Sampler app (iOS or Desktop) and load the .dslibrary file.

🎛 Controls

Reverb: Adjusts the spatial depth and hall ambience.

Attack: Controls the onset speed.

Default is set to 0.001s for instant response.

Release: Sets the fade-out duration after the key is released.

Tone: Adjusts the brightness of the sound (Low-pass Filter).

🤝 Credits & Sources
Original Audio & Image Source: National Gugak Center ([국립국악원](https://www.gugak.go.kr/))
Developed by: jonijonii
Assisted by: Gemini
