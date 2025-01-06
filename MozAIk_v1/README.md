
![MozAIk_v1 4_gh-pic-no-wf](https://github.com/user-attachments/assets/82ebb146-d65f-4395-84b6-0d272b9d9069)

### Setup Guide:

Install Mixxx: https://mixxx.org/download/

Install ComfyUI: https://github.com/comfyanonymous/ComfyUI/releases

Install [Manager](https://github.com/ltdrdata/ComfyUI-Manager), [AnimateDiff Evolved](https://github.com/Kosinkadink/ComfyUI-AnimateDiff-Evolved) and [VideoHelperSuite](https://github.com/Kosinkadink/ComfyUI-VideoHelperSuite) (Start with the Manager).

Download [MozAIk_v1.4.json](https://github.com/GomuSkelly/MozAIk/blob/main/MozAIk_v1/MozAIk_v1.4.json) and with ComfyUI open, drag the .json file into the browser window.

The MozAIk intro video used the prompt "160bpm trap heaven church dubstep jungle". Copy this prompt and paste it where you can see the supplied prompt "laughing". This generates audio that mostly has either 80/160 bpm (*even with "160bpm" in the prompt, some generations have a random bpm - hide/delete these from the Mixxx Library).

After generating your first .mp4 in ComfyUI with MozAIk_v1.4.json, open Mixxx and navigate via the Library to the "audio" folder inside ComfyUI > outputs.

Right click on the "audio" folder and select "Add to Quick Links" and from the same menu also select "Add to Library".

You will now be able to see the newly generated .mp4's under "Tracks" in the Library when opening Mixxx.

On Windows, Ctrl+Shift+L rescans the Library for new audio material as it is being generated.

In Mixxx, right click on the generated audio under "Tracks", and select "Analyse".

Select all files generated with the above example prompt that have 80/160 bpm, and drag them to "Auto DJ".

The Auto DJ fade mode should be set to "Full Intro + Outro" with the transition duration set to 23.

On Windows, Shift+F12 enables Auto DJ.

### Specifications for MozAIk v1.4:

The small demo video released Jan 1st was created with a 4060TI 16GB.

Running ComfyUI, Mixxx, OBS (recording@4k), generations take around 30 seconds with looping video artwork, and approx. 14 seconds for static artwork.

ComfyUI audio generation and Mixxx has been tested (without artwork generation) in audio effects heavy setups on a laptop with 4060 8GB card and 16GB system RAM.

If you're testing and have success on lower spec hardware, let us know!
