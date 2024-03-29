# Visual Data-Type Understanding does not emerge from Scaling Vision-Language Models

Official code for the ICLR'24 paper ["Visual Data-Type Understanding does not emerge from Scaling Vision-Language Models"](https://arxiv.org/abs/2310.08577). Authors: [Vishaal Udandarao](https://vishaal27.github.io/)\*, [Max F. Burg](https://scholar.google.de/citations?user=-T_5tc0AAAAJ&hl=en)\*, [Samuel Albanie](https://samuelalbanie.com/)§, and [Matthias Bethge](https://bethgelab.org/)§.

\* Equal contribution. Author ordering decided by coin flip.  § Joint senior authors.

# Introduction
Recent advances in the development of vision-language models (VLMs) are yielding remarkable success in recognizing visual semantic content, including impressive instances of compositional image understanding. Here, we introduce the novel task of _Visual Data-Type Identification_, a basic perceptual skill with implications for data curation (e.g., noisy data-removal from large datasets, domain-specific retrieval) and autonomous vision (e.g., distinguishing changing weather conditions from camera lens staining). We develop two datasets consisting of animal images altered across a diverse set of 27 visual _data-types_, spanning four broad categories. An extensive zero-shot evaluation of 39 VLMs, ranging from 100M to 80B parameters, shows a nuanced performance landscape. While VLMs are reasonably good at identifying certain stylistic _data-types_, such as cartoons and sketches, they struggle with simpler _data-types_ arising from basic manipulations like image rotations or additive noise. Our findings reveal that (i) model scaling alone yields marginal gains for contrastively-trained models like CLIP, and (ii) there is a pronounced drop in performance for the largest auto-regressively trained VLMs like OpenFlamingo. This finding points to a blind spot in current frontier VLMs: they excel in recognizing semantic content but fail to acquire an understanding of visual _data-types_ through scaling. By analyzing the pre-training distributions of these models and incorporating _data-type_ information into the captions during fine-tuning, we achieve a significant enhancement in performance. By exploring this previously uncharted task, we aim to set the stage for further advancing VLMs to equip them with visual data-type understanding.

# Getting started
Stay tuned! Code and datasets will be updated soon!

# SyntheticTypeIdent
The SyntheticTypeIdent dataset can be found here: https://huggingface.co/datasets/bethgelab/SyntheticTypeIdent
