# UCU Audio Processing Course

# Setup Working Environment  

## Pre-requirements 

- [Poetry](https://python-poetry.org/docs/#installation).
- VS Code — [Ubuntu](https://code.visualstudio.com/docs/setup/linux), [macOS](https://code.visualstudio.com/docs/setup/mac) and [Windows](https://code.visualstudio.com/docs/setup/windows) installation guides.
- (Optional) CUDA Version: 11.4; Driver Version: 470.129.06 — [Installation](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html).

## Setup environment 

1. Install Poetry using [Poetry full guide](https://python-poetry.org/docs/#installation).
    > **Important**: Check if it is working using `poetry --version`.
2. Run command to keep your `.venv` folder right in your project: `poetry config virtualenvs.in-project true`
3. `poetry shell`.
    > **Important**: If you have `conda` and 2 environments were activated: `conda deactivate`.
4. `poetry install --no-root`.

In order to activate environment on the next use:

`poetry shell`

> **Important**: you should be inside your project folder to do it.

# Start Jupyter

```bash
jupyter lab --port 7766
```

> **Note**: you may use any port.

# Content 

1. [x] Intro in Audio ML. Basic Audio Processing. Self Supervised Representations
    1. [x] Intro in Audio ML. Digital wave representation. Spectral audio representation
        - Author: Volodymyr, Andrii
        - Recording: 
    2. [x] Pre-processing, Filtering, Clustering
        - Author: Oles, Andrii
        - Colab: https://colab.research.google.com/drive/1PaM4K2eJoqeC8s0JLiiJ7RrDFI56rSxn?usp=sharing
        - Recording:
    3. [x] Self Supervised Representations
        - Author: Volodymyr, Andrii
        - Recording:
2. [] Audio Classification and Detection. Validation
    1. [x] Basic Audio Classification model
        - Author: Volodymyr, Andrii
        - Kaggle Inference: https://www.kaggle.com/code/vladimirsydor/ucu-hms-inference/notebook
        - Recording: 
    2. [x] Validation 
        - Author: Anton, Andrii
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

1. Create a [Kaggle](https://www.kaggle.com/) account.
2. Create a [Notebook](https://www.kaggle.com/code).
3. Explore the [docs](https://www.kaggle.com/docs/notebooks) and find out how to:
    - Add the Kaggle dataset to the notebook.
    - Turn on GPU.

## Colab 

1. Create a Notebook in [Colab](https://colab.research.google.com/).
2. Enable GPU.
3. Add the Kaggle dataset to Colab following the [guide](https://www.geeksforgeeks.org/how-to-import-kaggle-datasets-directly-into-google-colab/).

# Data

TODO

## How to use Kaggle datasets

1. Create a [Kaggle](https://www.kaggle.com/) account.
2. Proceed [with Installation & Authentication](https://www.kaggle.com/docs/api#getting-started-installation-&-authentication).
3. Don't forget to join a competition and accept its rules on a Kaggle website.
4. Download the dataset with an API command.

# Feedback [Only For Lectors]

TODO

# Citation

```
@misc{ucu_audio_processing_course_2024,
  author = {Volodymyr Sydorskyi, Anton Bazdyrev, Oles Dobosevych, Andrii Shevtsov},
  title = {UCU Audio Processing Course 2024},
  year = {2024},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/VSydorskyy/ucu_audio_processing_course}},
}
```
