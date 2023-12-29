# UCU Audio Processing Course

# Setup Working Environment  

## Pre-requirements 

- [Poetry 1.5.1](https://python-poetry.org/docs/#installation)
- VS Code - [Ubuntu Installation](https://code.visualstudio.com/docs/setup/linux)
- (Optional) CUDA Version: 11.4; Driver Version: 470.129.06 - [Installation](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html)

## Setup environment 

1. Install Poetry using [Poetry full guide](https://python-poetry.org/docs/#installation).
    - Important: Check if it is working using `poetry --version`
2. Run command to keep your `.venv` folder right in your project: `poetry config virtualenvs.in-project true`
3. `poetry shell`
    - Important: If you have `conda` and 2 environments were activated: `conda deactivate`
4. `poetry install --no-root`

In order to activate environment on the next use. Important: you should be inside your project

`poetry shell`

# Start Jupyter

You may use any port 
```bash
jupyter lab --port 7766
```

# Content 

1. [] Basic Audio Processing and Self Supervised Representations
    1. [] Digital wave representation. Waveform and Spectral Domains
        - Author: 
        - Recording: 
    2. [] Pre-processing, Filtering, Clustering
        - Author: 
        - Recording:
    3. [] Self Supervised Representations
        - Author: 
        - Recording:
2. [] Audio Classification and Detection. Validation
    1. [] Basic Audio Classification model
        - Author: 
        - Recording: 
    2. [] Validation 
        - Author: 
        - Recording:
    3. [] Speaker diarization 
        - Author: 
        - Recording:
3. [] ASR
    1. [] Data Preparation
        - Author: 
        - Recording:
    2. [] Modelling
        - Author: 
        - Recording:
    3. [] Modelling
        - Author: 
        - Recording:
4. [] TTS
    1. [] Introduction into Generative Models
        - Author: 
        - Recording:
    2. [] Modelling
        - Author: 
        - Recording:
    3. [] Modelling
        - Author: 
        - Recording:

# Use Kaggle or Colab for computations

## Kaggle 

1. Create [Kaggle](https://www.kaggle.com/) account 
2. Create [Notebook](https://www.kaggle.com/code)
3. Explore [docs](https://www.kaggle.com/docs/notebooks) and find out how 
    - Add Kaggle dataset to notebook 
    - Turn on GPU 

## Colab 

1. Create Notebook in [Colab](https://colab.research.google.com/)
2. Enable GPU 
3. Add Kaggle dataset to Colab - https://www.geeksforgeeks.org/how-to-import-kaggle-datasets-directly-into-google-colab/

# Data

TODO

## How to use Kaggle datasets

1. Create [Kaggle](https://www.kaggle.com/) account
2. Proceed [with Installation & Authentication](https://www.kaggle.com/docs/api#getting-started-installation-&-authentication)
3. Don't forget to join a competition and accept its rules on a Kaggle website.
4. Download dataset with API command 

# Feedback [Only For Lectors]

TODO

# Citation

```
@misc{ucu_audio_processing_course_2024,
  author = {Sydorskyi Volodymyr, Bazdyrev Anton, Oles Dobosevych},
  title = {UCU Audio Processing Course 2024},
  year = {2024},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/VSydorskyy/ucu_audio_processing_course}},
}
```
