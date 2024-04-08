# UCU Audio Processing Course

# Setup Working Environment  

## Pre-requirements 

- [Poetry](https://python-poetry.org/docs/#installation).
- VS Code — [Ubuntu](https://code.visualstudio.com/docs/setup/linux), [macOS](https://code.visualstudio.com/docs/setup/mac) and [Windows](https://code.visualstudio.com/docs/setup/windows) installation guides.
- (Optional) CUDA Version: 11.4; Driver Version: 470.129.06 — [Installation](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html).

### Pytorch base knoweledge 

Course will be using Python and Pytorch as main Deep Learning Framework. So it is essential to have basic Pytorch knowledge and a bit of hands-on experience

In order to update or gain this knowledge you can use list of next tutorials and resources:
- [Official Pytorch Tutorials](https://pytorch.org/tutorials/)
- [Stanford Pytorch Tutorials](https://web.stanford.edu/class/archive/cs/cs224n/cs224n.1214/materials/CS224N_PyTorch_Tutorial.html)
- [Repository with different Pytorch Tutorials](https://github.com/yunjey/pytorch-tutorial)
- [Detailed example of Sequence Classification and NER](https://github.com/VSydorskyy/iasa_nlp_course/blob/main/Lecture_4/Recurrent_models.ipynb)

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
2. [x] Audio Classification and Detection. Validation
    1. [x] Basic Audio Classification model
        - Author: Volodymyr, Andrii
        - Kaggle Inference: https://www.kaggle.com/code/vladimirsydor/ucu-hms-inference/notebook
        - Processed Data: https://www.kaggle.com/datasets/vladimirsydor/ucu-hms-h5py/data
        - Recording: 
    2. [x] Validation 
        - Author: Anton, Andrii
        - Recording:
    3. [x] Speaker diarization 
        - Author: Anton, Andrii
        - Recording:
3. [x] ASR
    1. [x] Introduction to ASR
        - Author: Oles
        - Colab: https://colab.research.google.com/drive/1iJvuurEQDaOkBba2zm1DSEkcdNDGhmU4
        - Recording:
    2. [x] Deeper ASR overview. CTC loss and Encoder architecture for ASR
        - Author: Yurii, Volodymyr
        - Recording:
    3. [x] introduction into Transformers. Whisper
        - Author: Yurii, Andrii
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
  author = {Volodymyr Sydorskyi, Anton Bazdyrev, Oles Dobosevych, Yurii Laba, Andrii Shevtsov},
  title = {UCU Audio Processing Course 2024},
  year = {2024},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/VSydorskyy/ucu_audio_processing_course}},
}
```
