<h1 align="center">
  <!-- <br>
  <a href="http://www.amitmerchant.com/electron-markdownify"><img src="https://raw.githubusercontent.com/amitmerchant1990/electron-markdownify/master/app/img/markdownify.png" alt="Markdownify" width="200"></a>
  <br> -->
  🔥(ICLR 2025) One-Prompt-One-Story: Free-Lunch Consistent Text-to-Image Generation Using a Single Prompt
  <br>
</h1>


<div align="center">

<a href="http://3090-v6.byliutao.xyz:7860" style="display: inline-block;">
    <img src="./resource/gradio.svg" alt="demo" style="height: 20px; vertical-align: middle;">
</a>&nbsp;
<a href="https://arxiv.org/abs/2501.13554" style="display: inline-block;">
    <img src="https://img.shields.io/badge/arXiv%20paper-2406.06525-b31b1b.svg" alt="arXiv" style="height: 20px; vertical-align: middle;">
</a>&nbsp;
<a href="https://byliutao.github.io/1Prompt1Story.github.io/" style="display: inline-block;">
    <img src="https://img.shields.io/badge/Project_page-More_visualizations-green" alt="project page" style="height: 20px; vertical-align: middle;">
</a>&nbsp;

</div>



<p align="center">
  <a href="#key-features">Key Features</a> •
  <a href="#how-to-use">How To Use</a> •
  <a href="#license">License</a> •
  <a href="#Citation">Citation</a> 
</p>

<p align="center">
  <img src="./resource/photo.gif" alt="screenshot" />
</p>


## Key Features

* Consistent Identity Image Generation.
* Gradio Demo.
* Consistory+ Benchmark: contains 200 prompt sets, with each set containing between 5 and 10 prompts, categorized into 8 superclasses: humans, animals, fantasy, inanimate, fairy tales, nature, technology.
* Benchmark Generation Code.


## How To Use

```bash
# Clone this repository
$ git clone https://github.com/byliutao/1Prompt1Story

# Go into the repository
$ cd 1Prompt1Story

### Install dependencies ###
$ conda create --name 1p1s python=3.10
$ conda activate 1p1s
# choose the right cuda version of your device
$ conda install pytorch torchvision torchaudio pytorch-cuda=12.1 -c pytorch -c nvidia 
$ conda install conda-forge::transformers 
$ conda install -c conda-forge diffusers
$ pip install opencv-python scipy gradio=4.44.1 sympy==1.13.1
### Install dependencies ENDs ###

# Run sample code
$ python main.py

# Run gradio demo
$ python app.py

# Run Consistory+ benchmark
$ python -m resource.gen_benchmark --save_dir ./result/benchmark --benchmark_path ./resource/consistory+.yaml
```

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.


## Citation
If our work assists your research, feel free to give us a star ⭐ or cite us using:
```
@inproceedings{
anonymous2025onepromptonestory,
title={One-Prompt-One-Story: Free-Lunch Consistent Text-to-Image Generation Using a Single Prompt},
author={Anonymous},
booktitle={The Thirteenth International Conference on Learning Representations},
year={2025},
url={https://openreview.net/forum?id=cD1kl2QKv1}
}
```
