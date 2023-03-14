# OxCrest Generator

Use machine learning to generate a new Oxford college crest design based on a given prompt.

This is a project built for [Hack Cambridge Spyder Lite](https://hack-cambridge-spyder-lite.devpost.com/?ref_feature=challenge&ref_medium=discover). Check our [Devpost](https://devpost.com/software/oxcrest-generator) here. 

## Inspiration

College puffers are an essential part of the Oxbridge experience. Many students wear puffers showing their college's crests as a way of expression. But what if your college's crest is just too ugly? 

In this project, we created a machine learning program which is able to generate a college crest based on a given prompt, in order to make the most unique and fashionable college puffer. 

## Implementation

[Dreambooth stable diffusion ](https://github.com/XavierXiao/Dreambooth-Stable-Diffusion) was used to train a text to image generation model using Oxford University's 44 college crests. 

This was combined with a [ControlNet made by lllyasviel on Hugging Face](https://huggingface.co/lllyasviel/sd-controlnet-scribble) to restrict the shape of the image generation into a shield crest shape.

Further efforts were made using [OpenCV](https://opencv.org/) in order to automate the detection and replacement of crests in photos of college puffers, although it is yet to be functional. 

## Usage

Run the Jupyter Notebook [OxCrest.ipynb](https://github.com/shinben0327/OxCrest-Generator/blob/main/OxCrest.ipynb) following its instructions. 

Make sure to login using a [Hugging Face token](https://huggingface.co/docs/hub/security-tokens) for model access, which can be obtained for free with a Hugging Face account. 

The prompt may be changed for different results.
```python
prompt = "a photo of an oxford college crest that includes a shape of a cat"
```

## Examples

Using the prompt above, example results have been generated. 

![Best Results](https://github.com/shinben0327/OxCrest-Generator/blob/main/examples/best_results.png?raw=true)
