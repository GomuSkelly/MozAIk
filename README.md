# MozAIk
**Generative A\VJ System**

MozAIk v1 wf is a barebones implementation in ComfyUI for audio/artwork generation. Combined with the Mixxx DJing software, it constitutes the realtime generative DJing aspect of MozAIk's A\VJ system. 


![MozAIk](https://github.com/user-attachments/assets/64cf2bcf-6e3b-403e-bced-e89ba1f27cee)

https://github.com/user-attachments/assets/aeb8d03f-1225-4dec-91bc-5e8eca3f3989



**2025-01-01 MozAIk v1 released.**

Quick Demo: https://www.youtube.com/watch?v=hdIFKt8geU8



**Setup Guide:**

Install Mixxx: https://mixxx.org/download/ 

Install ComfyUI: https://github.com/comfyanonymous/ComfyUI/releases

Install [Manager](https://github.com/ltdrdata/ComfyUI-Manager), [AnimateDiff Evolved](https://github.com/Kosinkadink/ComfyUI-AnimateDiff-Evolved) and [VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite) (Start with the Manager).

Download [MozAIk_v1.1.json 
](https://github.com/GomuSkelly/MozAIk/blob/main/MozAIk_v1.1.json
) and with ComfyUI open, drag the .json file into the browser window.

The MozAIk intro video used the prompt "160bpm trap heaven church dubstep jungle". Copy this prompt and paste it where you can see the supplied prompt "laughing".

This generates audio that mostly has either 80/160 bpm although there are also generations that have other random bpm.

After generating your first .mp4 in ComfyUI with MozAIk_v1.1.json, open Mixxx and navigate via the Library to the "audio" folder inside ComfyUI > outputs. 

Right click on the "audio" folder and select "Add to Quick Links" and from the same menu also select "Add to Library". 

You will now be able to see the newly generated .mp4's under "Tracks" in the Library when opening Mixxx.

On Windows, Ctrl+Shift+L rescans the Library for new audio material as it is being generated.

In Mixxx, right click on the generated audio under "Tracks", and select "Analyse". 

Select all files generated with the above example prompt *that have 80/160 bpm*, and copy them to "Auto DJ". 

The Auto DJ fade mode should be set to "Full Intro + Outro" with the transition duration set to **23**. 

On Windows, Shift+F12 enables Auto DJ.



**Specifications for MozAIk v1.1:**

The small demo video released Jan 1st was created with a 4060TI 16GB. 

Running ComfyUI, Mixxx, OBS (recording@4k), generations take around 30 seconds with looping video artwork, and approx. 14 seconds for static artwork. 

ComfyUI audio generation and Mixxx has been tested (without artwork generation) in audio effects heavy setups on a laptop with 4060 8GB card and 16GB system RAM.

If you're testing and have success on lower spec hardware, let us know!

Tested with Mixxx 2.4.1, if you have any issues with 2.5.0, please report back.



**Models:**

All necessary model links are now in the notes of our workflows. (Contained within the MozAIk_v1.1.json and upcoming wf's)


For the initial release, a limited amount of custom nodes were used to ensure the core of MozAIk's audio system can be set up without many complications for beginners. 

In the days ahead, there will be more complex workflows released. Today we release a basic template, and plant the seed of MozAIk.

Have fun!
