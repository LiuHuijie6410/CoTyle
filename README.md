
# A Style is Worth One Code: Unlocking Code-to-Style Image Generation with Discrete Style Space
<p align="center"> 
<a href="xxx"><img alt="Build" src="https://img.shields.io/badge/Project%20Page-Homepage-yellow"></a> 
<a href="xxx"><img alt="Build" src="https://img.shields.io/badge/GitHub-Code-f8f0f0.svg"></a> 
<a href="xxx"><img alt="Build" src="https://img.shields.io/badge/arXiv-Paper-da282a.svg"></a>
<a href="https://huggingface.co/spaces/Kwai-Kolors/CoTyle"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Demo-fd8b02"></a>
</p>

<p align="center">
    <span style="color:#137cf3; font-family: Gill Sans">Huijie Liu</span><sup>1,2</sup>,
    <span style="color:#137cf3; font-family: Gill Sans">Shuhao Cui</span><sup>1</sup>,
    <span style="color:#137cf3; font-family: Gill Sans">Haoxiang Cao</span><sup>1,3</sup>,
    <span style="color:#137cf3; font-family: Gill Sans">Shuai Ma</span><sup>1</sup>,
    <span style="color:#137cf3; font-family: Gill Sans">Bing Yu</span><sup>1</sup>,
    <span style="color:#137cf3; font-family: Gill Sans">Kai Wu</span><sup>1,†</sup>,
    <span style="color:#137cf3; font-family: Gill Sans">Guoliang Kang</span><sup>2,†</sup>
    <br>
    <sup>1</sup><span style="font-size: 16px">Kolors Team, Kuaishou Technology</span>, 
    <sup>2</sup><span style="font-size: 16px">Beihang University</span>,
    <sup>3</sup><span style="font-size: 16px">South China Normal University</span>
    <br>
    <sup>†</sup><span style="font-size: 16px">Co-Corresponding Author</span>
</p>

## 🔥 News
- [10/16/2025] 🔥 The [homepage](xxx) of CoTyle is released.
- [10/16/2025] 🔥 The [paper](xxx) of CoTyle is released on Arxiv.
- [10/16/2025] 🔥 The [demo](https://huggingface.co/spaces/Kwai-Kolors/CoTyle) of CoTyle is launched on Huggingface Space.

## 📝 ToDo
- [x] Publish the paper on Arxiv.
- [x] Release the homepage of CoTyle.
- [x] Launch a free demo on Hugging Face Spaces.
- [ ] Open source the code and model weights.

## 📖 Abstract
Innovative visual stylization is a cornerstone of artistic creation, while generating and representing novel styles remains a persistent challenge.Existing generative methods often rely on style images, lengthy textual descriptions, or parameter-efficient fine-tuning (PEFT) to guide models in generating images with specific styles. However, these methods struggle to create novel styles and require complex representations to convey stylistic information.In this paper, we affirm that a style is worth one numerical code by introducing the novel task, code-to-style image generation, which produces images with novel, consistent visual styles conditioned solely on a style code.To date, this field has only been explored by the industry(e.g., Midjourney), with no open-source research from the academic community.Specifically, we train a discrete style codebook to extract style embeddings from reference images. These embeddings then condition a T2I-DM to generate an image that aligns with the reference style.Specifically, we first train a discrete style codebook to extract style representations from reference images.Then, we train a text-to-image diffusion model (T2I-DM) conditioned on the output of the codebook, enabling it to generate images with specific style.Using the style codebook, we encode a large set of style images into indices and train an autoregressive model on them to model their distribution, which acts as the style generator.During inference, a numerical code deterministically samples a novel sequence of indices from the transformer. This sequence is then condition the diffusion process, generating style images.Unlike existing methods, our approach offers unparalleled simplicity and diversity, unlocking a vast space of reproducible styles from minimal input.Extensive experiments validate that SeeTyle effectively turns a single code into a powerful style controller, demonstrating a style is worth one code.

## ⚡️ Quick Start
We have first launched a [demo](https://huggingface.co/spaces/Kwai-Kolors/CoTyle) on HuggingFace Space—-feel free to try it out! 
The code will be released by mid-November.

