![MozAIk_Generative-Sampler_v1_gh-pic-no-wf](https://github.com/user-attachments/assets/760e7e23-4aa9-4556-bfe3-e7d2a771b63c)

Follow [this guide](https://github.com/GomuSkelly/MozAIk/edit/main/README.md), then install [cg-use-everywhere](https://github.com/chrisgoringe/cg-use-everywhere) nodes via the Manager in ComfyUI.

Download [MozAIk_Generative-Sampler_v1.1.json](https://github.com/GomuSkelly/MozAIk/blob/main/MozAIk_Generative-Sampler/MozAIk_Generative-Sampler_v1.1.json) and with ComfyUI open, drag the .json file into the browser window.

On a 4060TI 16GB, the generative sampler takes just under 10 mins to create a full 64 clip sample bank (at 47.6s per sample length).

It's possible to change the length of the samples generated

YMMV with samples shorter/longer than 47.6s. Some prompts work really well with a few seconds sample length and others sound garbled.

