## tutorial on noise and/or artifacts removal using convolution neural network

The tutorial is currently composed of three notebooks: 

  - `cnn4denoise.ipynb` how to build and train a basic convolution neural networks to denoise a synthesized dataset
  - `mdl-prod-toy.ipynb` Assmue you train the model on a cluster or desktop that has an NVIDIA GPU and save your model to a file. THis notebook explains how to load the trained model and run it on your laptop to denoise your images.
  - `TomoGAN-prod.ipynb` explains how to train the more advanced TomoGAN for real scientific images, and use it in real world.
  
## Using the Notebooks

The notebooks are designed to be easy to use on the cloud or on your own systems.

### Try in on Binder

without installing anything locally.
[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/lzhengchun/dn-tutorial/HEAD)

### Running Locally

The environment needed for the notebook is described in [`environment.yml`](./environment.yml)

First, install [Anaconda](https://docs.anaconda.com/anaconda/install/) then use Anaconda's command line tool to build the environment:

```bash
conda env create --file environment.yml
```

### Running on Google Colab

- go to `https://colab.research.google.com/` then log in your Google account
- Try to go to `File -> Open` if the following box does not show up
- Hit the `GitHub` tab shown in the open box, then past `https://github.com/AIScienceTutorial/Denoising` as shown in the following screenshot and hit the search button
- Choose and hit a notebook that you want to run.
- play it and enjoy(hopefully)

![Colab-Open](img/colab.png) 

## Citation 
If you find this material useful for your research, please consider cite our paper(s):

- Zhengchun Liu, Tekin Bicer, Rajkumar Kettimuthu and Ian Foster, "Deep Learning Accelerated Light Source Experiments," 2019 IEEE/ACM Third Workshop on Deep Learning on Supercomputers (DLS), Denver, CO, USA, 2019, pp. 20-28, doi: 10.1109/DLS49591.2019.00008.

- Zhengchun Liu, Tekin Bicer, Rajkumar Kettimuthu, Doga Gursoy, Francesco De Carlo, and Ian Foster, "TomoGAN: low-dose synchrotron x-ray tomography with generative adversarial networks: discussion," J. Opt. Soc. Am. A 37, 422-434 (2020)

Or via bibtex
```
@inproceedings{liu2019deep,
    title={Deep Learning Accelerated Light Source Experiments},
    author={Zhengchun Liu and Tekin Bicer and Rajkumar Kettimuthu and Ian Foster},
    year={2019},
    booktitle={2019 IEEE/ACM Third Workshop on Deep Learning on Supercomputers (DLS)},
    pages={20--28},
    doi={10.1109/DLS49591.2019.00008}
}

@article{liu2020tomogan,
  title={TomoGAN: low-dose synchrotron x-ray tomography with generative adversarial networks: discussion},
  author={Liu, Zhengchun and Bicer, Tekin and Kettimuthu, Rajkumar and Gursoy, Doga and De Carlo, Francesco and Foster, Ian},
  journal={Journal of the Optical Society of America A},
  volume={37},
  number={3},
  pages={422--434},
  year={2020},
  doi={10.1364/JOSAA.375595},
  publisher={Optical Society of America}
}

```
