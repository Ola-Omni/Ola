<p align="center" width="100%">
<img src="https://ola-omni.github.io/static/images/ola-icon.png" alt="967023137dff29e65b21544e7620e0f7.webp" width=60%>
</p>
<div>

## Ola: Pushing the Frontiers of Omni-Modal Language Model

<p align="left">
    <a href='https://github.com/liuzuyan' target='_blank'>Zuyan Liu<sup>*,1,2</sup></a>&emsp;
    <a href='https://github.com/dongyh20/' target='_blank'>Yuhao Dong<sup>*,2,3</sup></a>&emsp;
    Jiahui Wang<sup>1</sup></a>&emsp;<br>
    <a href='https://liuziwei7.github.io/' target='_blank'>Ziwei Liu<sup>3</sup></a>&emsp;
    Winston Hu<sup>2</sup></a>&emsp;
    <a href='https://scholar.google.com/citations?user=TN8uDQoAAAAJ' target='_blank'>Jiwen Lu<sup>1,&#x2709</sup></a>&emsp;
   <a href='https://raoyongming.github.io/' target='_blank'>Yongming Rao<sup>2,1,&#x2709</sup></a>&emsp;
</p>


<p align="left"><sup>1</sup>Tsinghua University &ensp; <sup>2</sup>Tencent Hunyuan Research&ensp; <sup>3</sup>S-Lab, NTU&ensp; </p>

<p align="left"><sup>*</sup> Equal Contribution<sup>&ensp; &#x2709</sup>  Corresponding Author</p>

[![Ola](https://img.shields.io/badge/Rank_1-OpenCampass(<15B)-blue)](https://rank.opencompass.org.cn/leaderboard-multimodal/?m=REALTIME)    [![Ola](https://img.shields.io/badge/Rank_8-VideoMME-red)](https://video-mme.github.io/home_page.html#leaderboard) 

---

**Project Page:** [![Ola](https://img.shields.io/badge/Ola-project_page-orange)](https://ola-omni.github.io) 

**Weights in Huggingface:** [![hf_checkpoint](https://img.shields.io/badge/🤗-Ola_7b-green)](https://huggingface.co/THUdyh/Ola-7b)  [![hf_checkpoint](https://img.shields.io/badge/🤗-Ola_Image-green)](https://huggingface.co/THUdyh/Ola-Image)   [![hf_checkpoint](https://img.shields.io/badge/🤗-Ola_Video-green)](https://huggingface.co/THUdyh/Ola-Video)

**arXiv Paper:** [![arxiv](https://img.shields.io/badge/Arxiv-2502.04328-b31b1b.svg?logo=arXiv)](https://arxiv.org/abs/2502.04328)

**Demo by Gradio:** [![demo](https://img.shields.io/badge/Ola-Demo-yellow)](https://huggingface.co/spaces/THUdyh/Ola) 

**Training Data:** [![data](https://img.shields.io/badge/Ola-Data-purple)](https://huggingface.co/datasets/THUdyh/Ola-Data) 

**中文解读**: [![chinese](https://img.shields.io/badge/Ola-机器之心-cyan)](https://mp.weixin.qq.com/s/N4bjcHOejJudtxTFZVAXmg) 

Contact: Leave an issue or contact liuzuyan19@gmail.com . We are on call to respond.

## 📢 News

- 🔥[28/2/2025] We release the intermediate model, Ola-Image and Ola-Video, try building your own omni-modal models!

- 🚀[19/2/2025] We release the huggingface demo of Ola, try the advanced omni-modal model on your own!

- 🔥[18/2/2025] The training data, training script for Ola-7b is released!

- 🎉[07/2/2025] The Ola is released! Check our [project page](https://ola-omni.github.io), [model weights](https://huggingface.co/THUdyh/Ola-7b), [arXiv paper](https://arxiv.org/pdf/2502.04328) for the strong omni-modal understanding model!

- 🔥[06/2/2025] [Ola-7b](https://huggingface.co/THUdyh/Ola-7b) achieves **Rank #1** on the OpenCompass Multi-modal Leaderboard among all the models under 15B parameters with average score of **72.6**. Check the impressive results [here](https://rank.opencompass.org.cn/leaderboard-multimodal/?m=REALTIME)!

## 🚀Coming Soon

- [x] Evaluation code on omni-modal benchmarks
- [x] Gradio Demo
- [x] Training Data (Video, Audio, Cross-Modality)

## 🌟 Introduction

### Roads to Ola

<p align="center" width="100%">
<img src="https://ola-omni.github.io/static/images/road.png" alt="road.png" width=100%>
</p>
<div>

**Ola** is an Omni-modal language model that achieves competitive performance across image, video, and audio understanding compared to specialized counterparts. We conduct a comprehensive exploration of architectural design, data curation, and training strategies essential for building a robust omni-modal model.

<p align="center" width="100%">
<img src="https://ola-omni.github.io/static/images/teaser.png" alt="teaser.png" width=100%>
</p>
<div>

### Architecture

<p align="center" width="100%">
<img src="https://ola-omni.github.io/static/images/method.png" alt="method.png" width=100%>
</p>
<div>

Ola supports omni-modal inputs including text, image, video, and audio, capable of processing the inputs simultaneously with competitive performance on understanding tasks for all these modalities. Meanwhile, Ola supports user-friendly real-time streaming decoding for texts and speeches thanks to the text detokenizer and the speech decoder.

### Training Strategies

<p align="center" width="100%">
<img src="https://ola-omni.github.io/static/images/training.png" alt="training.png" width=100%>
</p>
<div>

We visualize the relationships among modalities in the left part. Speech acts as the connection between language and audio knowledge, while video constructs the bridge with highly relevant visual and audio information. Therefore, we design the progressive alignment training strategy from primary to periphery. Furthermore, we design the cross-modality video-audio data to better capture the relationships among modalities.

### Performance

<p align="center" width="100%">
<img src="https://ola-omni.github.io/static/images/results.png" alt="results.png" width=100%>
</p>
<div>

Ola achieves competitive performance across major multi-modal benchmarks when compared to state-of-the-art specialist-modal LLMs.

## Installation


#### 1. Clone this repository:
```bash
git clone https://github.com/Ola-Omni/Ola
cd Ola
```

#### 2. Install the required package:
```bash
conda create -n ola python=3.10 -y
conda activate ola
pip install --upgrade pip
pip install -e .
```
#### 3.Install additional packages for training cases

```bash
pip install -e ".[train]"
pip install flash-attn --no-build-isolation
```

## Model Zoo

We provide our checkpoints at [Huggingface](https://huggingface.co/collections/THUdyh/ola-67b8220eb93406ec87aeec37)

| Model | Link | Size | Modal |
|:---:|:---:|:---:|:---:|
|Ola-7b | [Huggingface](https://huggingface.co/THUdyh/Ola-7b) | 7B | Text, Image, Video, Audio |
|Ola-Image | [Huggingface](https://huggingface.co/THUdyh/Ola-Image) | 7B | Text, Image |
|Ola-Video | [Huggingface](https://huggingface.co/THUdyh/Ola-Video) | 7B | Text, Image, Video |


## Quick Start

1. Download `Ola-7b` from [Huggingface](https://huggingface.co/THUdyh/Ola-7b) or skip the step to using the online weights directly.

2. Download audio encoder from [Huggingface](https://huggingface.co/THUdyh/Ola_speech_encoders/tree/main) and put the weights `large-v3.pt` and `BEATs_iter3_plus_AS2M_finetuned_on_AS2M_cpt2.pt` under repo directory `path/to/Ola/`

3. Run `inference/infer.py`

- Text & Image Understanding

```
python3 inference/infer.py --image_path *.png,jpg --text user_instruction
```

- Text & Video Understanding

```
python3 inference/infer.py --video_path *.mp4 --text user_instruction
```

- Text & Audio Understanding

```
python3 inference/infer.py --audio_path *.wav,mp3 --text user_instruction
```

- Audio & Image Understanding

```
python3 inference/infer.py --audio_path *.png,jpg --audio_path *.wav,mp3
```

## Evaluation

You can evaluate Ola model with [VLMEvalKit](https://github.com/open-compass/VLMEvalKit) and [lmms-eval](https://github.com/EvolvingLMMs-Lab/lmms-eval).

## Training

### Data Preparation

Please refer to [DATA.md](https://github.com/Ola-Omni/Ola/blob/main/DATA.md) for instructions of customized finetuning or using the provided datasets. 

### Start Training

Please follow the script below to start training. Make sure you have created the correct datasets for fine-tuning. 

1. Finetuning Ola-7b Model:

```
bash ./scripts/finetune_ola.sh
```

2. Finetuning Ola-Image Model (Ola Stage1 or Stage2)

```
bash ./scripts/finetune_ola_image.sh
```

3. Finetuning Ola-Video Model (Ola Stage3):

```
bash ./scripts/finetune_ola_video.sh
```

## Citation

If you find it useful for your research and applications, please cite our paper using this BibTeX:
```bibtex
@article{liu2025ola,
title={Ola: Pushing the Frontiers of Omni-Modal Language Model with Progressive Modality Alignment},
author={Liu, Zuyan and Dong, Yuhao and Wang, Jiahui and Liu, Ziwei and Hu, Winston and Lu, Jiwen and Rao, Yongming},
journal={arXiv preprint arXiv:2502.04328},
year={2025}
}
```

## Acknowledgement

- Our codebase is conducted on [LLaVA](https://github.com/LLaVA-VL/LLaVA-NeXT)

- Thanks [VLMEvalKit](https://github.com/open-compass/VLMEvalKit) and [lmms-eval](https://github.com/EvolvingLMMs-Lab/lmms-eval) team for the evaluation system!
