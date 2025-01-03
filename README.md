# MozAIk
**Generative A\VJ System**

MozAIk v1 wf is a barebones implementation in ComfyUI for audio/artwork generation. Combined with the Mixxx DJing software, it constitutes the realtime generative DJing aspect of MozAIk's A\VJ system. 


![MozAIk](https://github.com/user-attachments/assets/64cf2bcf-6e3b-403e-bced-e89ba1f27cee)

https://github.com/user-attachments/assets/aeb8d03f-1225-4dec-91bc-5e8eca3f3989



**2025-01-01 MozAIk v1 released.**

Quick Demo: https://www.youtube.com/watch?v=hdIFKt8geU8



Setup Guide *to follow* (messy draft guide being fleshed out presently)


Minimum Specifications for MozAIk v1 *to follow* (more testing on older devices required)


The small demo video released Jan 1st was created with a 4060TI 16GB. Running ComfyUI, Mixxx, OBS (recording@4k) generations take around 30 seconds with looping video artwork, and approx. 14 seconds for static artwork. ComfyUI audio generation and Mixxx has been tested (without artwork generation) in audio effects heavy setups on a laptop with 4060 8GB card and 16GB system RAM, and plays without issue for hours. A desktop 3060 12GB and laptop 2060 6GB will be used for testing to establish minimum spec. In the meantime, if you're testing and have success on lower spec hardware, let us know!

Install Mixxx: https://mixxx.org/download/ Install ComfyUI: https://github.com/comfyanonymous/ComfyUI/releases, download the MozAIk workflow, and check back in the hours ahead for detailed instructions.

Tested with Mixxx 2.4.1, if you have any issues with 2.5.0, please report back.

After installing ComfyUI, install the [Manager](https://github.com/ltdrdata/ComfyUI-Manager), [AnimateDiff Evolved](https://github.com/Kosinkadink/ComfyUI-AnimateDiff-Evolved) and [VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite) custom nodes (start with the Manager).

**AUDIO GENERATION Group**

Download [stable_audio_open_1.0.safetensors](https://huggingface.co/audo/stable-audio-open-1.0/blob/main/model.safetensors) and place in ComfyUI > models > checkpoints folder. Download "t5_base.safetensors" from the Model Manager. 

**STATIC ARTWORK MP4 FOR MIXXX Group**

The lcm LoRA "pytorch_lora_weights.safetensors" and "vae-ft-mse-840000-ema-pruned.safetensors" can be downloaded via the Model Manager.

**DYNAMIC ARTWORK MP4 FOR MIXXX Group** 

Download and place [animatediff_lightning_4step_comfyui.safetensors](https://huggingface.co/ByteDance/AnimateDiff-Lightning/blob/main/animatediff_lightning_4step_comfyui.safetensors) in the ComfyUI > models > animatediff_models folder.

Artwork generation models used in the demo video: [DreamShaper 8](https://civitai.com/models/4384) [Pixel Sorting](https://civitai.com/models/57963?modelVersionId=128713) [J.R. "Bob" Dobbs - v1.0](https://civitai.com/models/74788?modelVersionId=79532)

After generating your first .mp4 in ComfyUI with MozAIk_v1.json, open Mixxx and navigate via the Library to the "audio" folder inside ComfyUI > outputs. Right click on the "audio" folder and select "Add to Quick Links" and from the same menu also select "Add to Library". You will now be able to see the newly generated .mp4's under "Tracks" in the Library, and (on Windows) can use the shortcut Ctrl+Shift+L to rescan the Library as new audio material is being generated. 

The MozAIk intro video used the prompt "160bpm trap heaven church dubstep jungle". This generates audio that mostly has either 80/160 bpm although there are also generations that have other random bpm.

In Mixxx, right click on the generated audio under "Tracks", and select "Analyse". Select all files generated with the above example prompt *that have 80/160 bpm*, and copy them to "Auto DJ". The Auto DJ fade mode should be set to "Full Intro + Outro" with the transition duration set to 23. Shift+F12 enables Auto DJ.

For the initial release, a limited amount of custom nodes were used to ensure the core of MozAIk's audio system can be set up without many complications for beginners. 

In the days ahead, there will be more complex workflows released, and a video guide (and much better documentation!). Today we release a basic template, and plant the seed of MozAIk.

Have fun!


