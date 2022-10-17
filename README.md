# **GLIDE**

Repo for the project of **Neural Networks** 2022 based on the work [GLIDE: Towards Photorealistic Image Generation and Editing with Text-Guided Diffusion Models](https://arxiv.org/abs/2112.10741).

You can read the detailed work on the [Report](report.pdf).

For details on the pre-trained models in this repository, see the original [Model Card](model-card.md).

# **Usage**

## Online Notebooks

If you don't want to install this package you can run **GLIDE(filtered)** on these two Colab Notebooks: 

* The **C_Free&CLIP_guidance** [![][colab]][colab-text2im] notebook shows how to use GLIDE (filtered) with both classifier-free and CLIP guidance to produce images conditioned on text prompts. 
* The **inpaint** [![][colab]][colab-inpaint] notebook shows how to use GLIDE (filtered) to fill in a masked region of an image, conditioned on a text prompt.

[colab]: <https://colab.research.google.com/assets/colab-badge.svg>
[colab-text2im]: <https://colab.research.google.com/drive/107TfaoCr78kCrUqZPfW183nvT0ItramR?usp=sharing>
[colab-inpaint]: <https://colab.research.google.com/drive/1F35g0yIe1qATw6Tf-gVIQnBkyOEt9KIM?usp=sharing>

## Local notebooks
To install this package, clone this repository and then run:

```
pip install -e .
```

After meeting the requirements, see the [notebooks](notebooks) directory in order to run the **GLIDE(filtered)** model:

* The [text2im](notebooks/text2im.ipynb) notebook shows how to use GLIDE(filtered) with classifier-free guidance to produce images conditioned on text prompts. 
* The [inpaint](notebooks/inpaint.ipynb) notebook shows how to use GLIDE(filtered) to fill in a masked region of an image, conditioned on a text prompt. 
* The [clip_guided](notebooks/clip_guided.ipynb) notebook shows how to use GLIDE(filtered) + a filtered noise-aware CLIP model to produce images conditioned on text prompts.
