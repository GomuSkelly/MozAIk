# MozAIk
Generative A\VJ System

![MozAIk](https://github.com/user-attachments/assets/64cf2bcf-6e3b-403e-bced-e89ba1f27cee)

https://github.com/user-attachments/assets/aeb8d03f-1225-4dec-91bc-5e8eca3f3989

Setup Guide to follow.

Install Mixxx: https://mixxx.org/download/ Install ComfyUI: https://github.com/comfyanonymous/ComfyUI/releases, download the MozAIk workflow, and check back in the hours ahead for detailed instructions.

Tested with Mixxx 2.4.1, if you have any issues with 2.5.0, please report back.

After installing Mixxx, ComfyUI, the [Manager](https://github.com/ltdrdata/ComfyUI-Manager), [AnimateDiff Evolved](https://github.com/Kosinkadink/ComfyUI-AnimateDiff-Evolved) and [VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite), download "stable_audio_open_1.0.safetensors" and "t5_base.safetensors" from the Manager for the "AUDIO GENERATION" Group. 

For the "STATIC ARTWORK MP4 FOR MIXXX" Group, the lcm LoRA "pytorch_lora_weights.safetensors" and "vae-ftmse-840000-ema-pruned.safetensors" can be downloaded via the Manager.

For the "DYNAMIC ARTWORK MP4 FOR MIXXX" Group, place [animatediff_lightning_4step_comfyui.safetensors](https://huggingface.co/ByteDance/AnimateDiff-Lightning/blob/main/animatediff_lightning_4step_comfyui.safetensors) in the ComfyUI > models > animatediff_models folder.

Artwork generation models used in the demo video: [DreamShaper 8](https://civitai.com/models/4384) [Pixel Sorting](https://civitai.com/models/57963?modelVersionId=128713) [J.R. "Bob" Dobbs - v1.0](https://civitai.com/models/74788?modelVersionId=79532)
