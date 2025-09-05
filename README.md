# OneCAT: Decoder-Only Auto-Regressive Model for Unified Understanding and Generation

<div align="center">
  <img src="assets/banner.png" width="480" alt="onecat" />
</div>
<hr>

<div align="center" style="line-height: 1;">
  <a href="https://arxiv.org/abs/2509.03498" target="_blank" style="margin: 2px;">
    <img alt="Arxiv" src="https://img.shields.io/badge/OneCAT-Paper-red?logo=arxiv&logoColor=red"  fill-opacity="1" style="display: inline-block; vertical-align: middle;"/>
  </a>
  <a href="https://huggingface.co/onecat-ai" target="_blank" style="margin: 2px;">
    <img alt="Hugging Face" src="https://img.shields.io/badge/%F0%9F%A4%97%20OneCAT-Model-yellow" style="display: inline-block; vertical-align: middle;"/>
  </a>
  <a href="https://onecat-ai.github.io/" target="_blank" style="margin: 2px;">
    <img alt="Website" src="https://img.shields.io/badge/OneCAT-Website-0A66C2?logo=safari&logoColor=white" style="display: inline-block; vertical-align: middle;"/>
  </a>
</div>




## Brief Introduction
We introduce OneCAT, a unified multimodal model that seamlessly integrates understanding, generation, and editing within a novel, pure decoder-only transformer architecture. Our framework uniquely eliminates the need for external components such as Vision Transformers (ViT) or vision tokenizer during inference, leading to significant efficiency gains, especially for high-resolution
inputs. This is achieved through a modality-specific Mixture-of-Experts (MoE) structure trained with a single autoregressive (AR) objective, which also natively supports dynamic resolutions. Furthermore, we pioneer a multi-scale visual autoregressive mechanism within the Large Language Model (LLM) that drastically reduces decoding steps compared to diffusion-based methods while maintaining state-of-the-art performance. Our findings demonstrate the powerful potential of pure autoregressive modeling as a sufficient and elegant foundation for unified multimodal intelligence. As a result, OneCAT sets a new performance standard, outperforming existing open-source unified multimodal models across benchmarks for multimodal generation, editing, and understanding.

### Key Features

#### 🌟 Pure Decoder-Only Design

Eliminates external vision encoders and VAE tokenizers during inference, using only a lightweight patch embedding layer for raw image processing.


#### 🌟 Mixture-of-Experts (MoE)

Three specialized FFN experts: Text FFN for language comprehension, Understanding FFN for visual tokens, and Generation FFN for image synthesis.

#### 🌟 Multi-Scale Autoregressive
Pioneer Next Scale Prediction paradigm that generates images coarse-to-fine, drastically reducing generation steps compared to diffusion models.

For more details, please refer to the [***OneCAT Technical Report***](https://arxiv.org/abs/2509.03498).



## Contact
If you have any questions, you can either create issues or contact us by email wangyaoming03@meituan.com


## ✍️ Citation

```bibtex
@article{Li2025OneCAT,
  title   = {OneCAT: Decoder-Only Auto-Regressive Model for Unified Understanding and Generation},
  author  = {Han Li, Xinyu Peng, Yaoming Wang, Zelin Peng, Xin Chen, Rongxiang Weng, Jingang Wang, Xunliang Cai, Wenrui Dai, Hongkai Xiong},
  journal = {arXiv preprint arXiv:2509.03498},
  year    = {2025}
}
```

## 📜 License
OneCAT is licensed under the Apache 2.0.
