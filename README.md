
# A Style is Worth One Code: Unlocking Code-to-Style Image Generation with Discrete Style Space
<p align="center"> 
<a href="https://liuhuijie6410.github.io/OmniDish/"><img alt="Build" src="https://img.shields.io/badge/Project%20Page-OmniDish-yellow"></a> 
<a href="https://github.com/LiuHuijie6410/OmniDish"><img alt="Build" src="https://img.shields.io/badge/GitHub-OmniDish-f8f0f0.svg"></a> 
<a href="https://arxiv.org/abs/2504.09948"><img alt="Build" src="https://img.shields.io/badge/arXiv-OmniDish-da282a.svg"></a>
<a href="https://huggingface.co/datasets/liuhuijie6410/OmniDish-Edit-70K"><img src="https://img.shields.io/badge/%F0%9F%A4%97%20Hugging%20Face-Dataset-fd8b02"></a>
<a href="https://img.shields.io/badge/PDF-Appendix-da282a.svg"><img src="https://img.shields.io/badge/PDF-Appendix-d1cebc.svg"></a>
</p>

><p align="center"> <span style="color:#137cf3; font-family: Gill Sans">Huijie Liu</span><sup>1,2</sup>,</a>  <span style="color:#137cf3; font-family: Gill Sans">Bingcan Wang</span><sup>1</sup>,</a> <span style="color:#137cf3; font-family: Gill Sans">Jie Hu</span><sup>1</sup>,</a>  <span style="color:#137cf3; font-family: Gill Sans">Xiaoming Wei</span><sup>1</sup>, </a>  <span style="color:#137cf3; font-family: Gill Sans">Guoliang Kang</span><sup>2</sup></a> </a> <br> 
><span style="font-size: 16px">Meituan</span><sup>1</sup>, Beihang University</span><sup>2</sup></span></p>

<p align="center">
<img src="assets/fig1.png" width=95% height=95% 
class="center">
</p>

## 🔥 News
- [10/10/2025] 
- [10/10/2025] 🔥 The [homepage](https://liuhuijie6410.github.io/OmniDish/) of CoTyle is released.
- [10/10/2025] 🔥 The arXiv [paper](https://arxiv.org/abs/2504.09948) of CoTyle is released.

## 📖 Abstract
Innovative visual stylization is a cornerstone of artistic creation, while generating and representing novel styles remains a persistent challenge.Existing generative methods often rely on style images, lengthy textual descriptions, or parameter-efficient fine-tuning (PEFT) to guide models in generating images with specific styles. However, these methods struggle to create novel styles and require complex representations to convey stylistic information.In this paper, we affirm that a style is worth one numerical code by introducing the novel task, code-to-style image generation, which produces images with novel, consistent visual styles conditioned solely on a style code.To date, this field has only been explored by the industry(e.g., Midjourney), with no open-source research from the academic community.Specifically, we train a discrete style codebook to extract style embeddings from reference images. These embeddings then condition a T2I-DM to generate an image that aligns with the reference style.Specifically, we first train a discrete style codebook to extract style representations from reference images.Then, we train a text-to-image diffusion model (T2I-DM) conditioned on the output of the codebook, enabling it to generate images with specific style.Using the style codebook, we encode a large set of style images into indices and train an autoregressive model on them to model their distribution, which acts as the style generator.During inference, a numerical code deterministically samples a novel sequence of indices from the transformer. This sequence is then condition the diffusion process, generating style images.Unlike existing methods, our approach offers unparalleled simplicity and diversity, unlocking a vast space of reproducible styles from minimal input.Extensive experiments validate that SeeTyle effectively turns a single code into a powerful style controller, demonstrating a style is worth one code.

## ⚡️ Quick Start
We offer both CoTyle Commercial Edition and Open Source Edition. If you wish to directly use the highest-performing version of CoTyle, please proceed to xxx. If you are a professional developer and interested in further developing CoTyle, please follow the tutorial below.

### 🔧 Requirements and Installation

Install the requirements
```bash
git clone xxxxxxxxxtodo
cd xxxxxx
pip install -r requirements.txt
```

### ⏬ Download
Please download all the following models to the `./models` directory.

qwen image
CoTyle

### 🚄 Code-to-Style Generation

##  🌟 Citation
If CoTyle is helpful, please help to ⭐ the repo.

If you find this project useful for your research, please consider citing our paper:
```bibtex
@article{liu2025omni,
  title={xxx},
  author={xxx},
  journal={arXiv preprint arXiv:2504.09948},
  year={2025}
}
```

## Acknowledge
