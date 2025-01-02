# MozAIk
Generative A\VJ System

![MozAIk](https://github.com/user-attachments/assets/64cf2bcf-6e3b-403e-bced-e89ba1f27cee)

https://github.com/user-attachments/assets/aeb8d03f-1225-4dec-91bc-5e8eca3f3989

2025-01-01 MozAIk v1 released.

Setup Guide *to follow* (messy draft guide being fleshed out presently)


Minimum Specifications for MozAIk v1 *to follow* (more testing on older devices required)

The small demo video released Jan 1st was created with a 4060TI 16GB. Running ComfyUI, Mixxx, OBS (recording@4k) generations take around 30 seconds with looping video artwork, and approx. 14 seconds for static artwork. 

Install Mixxx: https://mixxx.org/download/ Install ComfyUI: https://github.com/comfyanonymous/ComfyUI/releases, download the MozAIk workflow, and check back in the hours ahead for detailed instructions.

Tested with Mixxx 2.4.1, if you have any issues with 2.5.0, please report back.

After installing Mixxx, ComfyUI, the [Manager](https://github.com/ltdrdata/ComfyUI-Manager), [AnimateDiff Evolved](https://github.com/Kosinkadink/ComfyUI-AnimateDiff-Evolved) and [VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite), download "stable_audio_open_1.0.safetensors" and "t5_base.safetensors" from the Manager for the "AUDIO GENERATION" Group. 

For the "STATIC ARTWORK MP4 FOR MIXXX" Group, the lcm LoRA "pytorch_lora_weights.safetensors" and "vae-ft-mse-840000-ema-pruned.safetensors" can be downloaded via the Manager.

For the "DYNAMIC ARTWORK MP4 FOR MIXXX" Group, place [animatediff_lightning_4step_comfyui.safetensors](https://huggingface.co/ByteDance/AnimateDiff-Lightning/blob/main/animatediff_lightning_4step_comfyui.safetensors) in the ComfyUI > models > animatediff_models folder.

Artwork generation models used in the demo video: [DreamShaper 8](https://civitai.com/models/4384) [Pixel Sorting](https://civitai.com/models/57963?modelVersionId=128713) [J.R. "Bob" Dobbs - v1.0](https://civitai.com/models/74788?modelVersionId=79532)

After generating your first .mp4 in ComfyUI with MozAIk_v1.json, open Mixxx and navigate via the Library to the "audio" folder inside ComfyUI > outputs. Right click on the "audio" folder and select "Add to Quick Links". You will now be able to see the newly generated .mp4's under "Tracks" in the Library, and (on Windows) can use the shortcut Ctrl+Shift+L to rescan the Library.

The MozAIk intro video used the prompt "160bpm trap heaven church dubstep jungle". This generates audio that mostly has either 80/160 bpm although there are also generations that have other random bpm.

In Mixxx, right click on the generated audio under "Tracks", and select "Analyse". Select all files generated with the above example prompt that have 80/160 bpm, and copy them to "Auto DJ". The Auto DJ fade mode should be set to "Full Intro + Outro" with the transition duration set to 23. Shift+F12 enables Auto DJ.

For the initial release, a limited amount of custom nodes were used to ensure the core of MozAIk's audio system can be set up without many complications for beginners. 

In the days ahead, there will be more complex workflows released, and a video guide (and much better documentation!). Today we release a basic template, and plant the seed of MozAIk.

Have fun!


