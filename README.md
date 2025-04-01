# UCU Audio Processing Course

# Setup Working Environment  

## Pre-requirements 

- [Poetry](https://python-poetry.org/docs/#installation).
- [Conda](https://conda.io/projects/conda/en/latest/user-guide/install/index.html). I advice using Miniconda
- VS Code — [Ubuntu](https://code.visualstudio.com/docs/setup/linux), [macOS](https://code.visualstudio.com/docs/setup/mac) and [Windows](https://code.visualstudio.com/docs/setup/windows) installation guides.
- (Optional) CUDA Version: 11.4; Driver Version: 470.129.06 — [Installation](https://docs.nvidia.com/cuda/cuda-installation-guide-linux/index.html).

### Pytorch base knoweledge 

Course will be using Python and Pytorch as main Deep Learning Framework. So it is essential to have basic Pytorch knowledge and a bit of hands-on experience

In order to update or gain this knowledge you can use list of next tutorials and resources:
- [Official Pytorch Tutorials](https://pytorch.org/tutorials/)
- [Stanford Pytorch Tutorials](https://web.stanford.edu/class/archive/cs/cs224n/cs224n.1214/materials/CS224N_PyTorch_Tutorial.html)
- [Repository with different Pytorch Tutorials](https://github.com/yunjey/pytorch-tutorial)
- [Detailed example of Sequence Classification and NER](https://github.com/VSydorskyy/iasa_nlp_course/blob/main/Lecture_4/Recurrent_models.ipynb)

### Other additional materials

- [Youtube Videos. Audio Signal Processing for Machine Learning](https://www.youtube.com/playlist?list=PL-wATfeyAMNqIee7cH3q1bh4QJFAaeNv0)

## Setup environment 

### Poetry (Main)

1. Install Poetry using [Poetry full guide](https://python-poetry.org/docs/#installation).
    > **Important**: Check if it is working using `poetry --version`.
2. Run command to keep your `.venv` folder right in your project: `poetry config virtualenvs.in-project true`
3. `poetry shell`.
    > **Important**: If you have `conda` and 2 environments were activated: `conda deactivate`.
    
    > If `poetry shell` returns *"The command "shell" does not exist."*, run `poetry self add poetry-plugin-shell` and try again ([source](https://python-poetry.org/docs/cli/#script-project:~:text=The%20shell%20command%20was%20moved%20to%20a%20plugin%3A%20poetry%2Dplugin%2Dshell)).
4. `poetry install --no-root`.

In order to activate environment on the next use:

`poetry shell`

> **Important**: you should be inside your project folder to do it.

### Conda (For TTS)

Next tutorial is mostly taken from [NeMo repo](https://github.com/NVIDIA/NeMo?tab=readme-ov-file#conda)

```bash
conda create --name nemo python==3.10.12
conda activate nemo
conda install pytorch torchvision torchaudio pytorch-cuda=11.8 -c pytorch -c nvidia
pip install Cython
pip install nemo_toolkit['all']
pip install jupyterlab
```

# Start Jupyter

```bash
jupyter lab --port 7766
```

> **Note**: you may use any port.

# Content 

1. [x] Intro in Audio. Basic Audio Processing
    1. [x] Intro in Audio ML. Digital wave representation. Spectral audio representation
        - Author: Volodymyr
        - Recording: https://youtu.be/qU3uiP2XSFg
    2. [x] Pre-processing, Filtering, Clustering
        - Author: Oles
        - Recording: https://youtu.be/LnCWHg6hn5o
    3. Homework
        - Google Form: https://forms.gle/kW9gGSocLyGTWLah6
        - Practical Task: Homework Section in https://github.com/VSydorskyy/ucu_audio_processing_course/blob/main/Module_1/Lecture_2/Pre_processing_Filtering_Clustering.ipynb
        - Deadline: 24.02.2025, 24:00 GMT +02:00
2. [x] Into to Pytorch. Basic Deep Learning Tasks
    1. [x] Validation 
        - Author: Anton and Volodymyr
        - Recording: https://youtu.be/HA4ZP3CH1UI
    2. [x] Intro to Basic Pytroch. CNNs. Image Classification
        - Author: Ostap
        - Recording: https://youtu.be/meRa1qNjQJs
    3. [x] Intro to Lightning. RNNs. Named Entity Recognition
        - Author: Anton
        - Recording: https://youtu.be/MG-dWWPDvQM
    4. [x] Self Supervised Audio Representations
        - Author: Yurii Yelisieiev 
        - Recording: https://youtu.be/5NyYP8oNbV8
    5. Homework
        - Google Form: https://forms.gle/4WHJourwLs29ZKYU8
        - Practical Task: Homework Section in https://github.com/VSydorskyy/ucu_audio_processing_course/blob/main/Module_2/Lecture_4/Self_Supervised_Representations.ipynb
        - Deadline: 07.04.2025, 24:00 GMT +02:00
3. [x] Audio Classification and Diarization
    1. [x] Audio Classification model
        - Author: Volodymyr
        - Recording: https://youtu.be/24Ee1LCDUNg
    2. Competition Alert !!!
        - Competition: https://www.kaggle.com/competitions/birdclef-2025/overview
        - Points: Bronze zone - 20 points; Silver zone - 40 points; Gold zone - 80 points
        - Deadline: 25.05.2025, 24:00 GMT +02:00
    3. [x] Speaker diarization 
        - Author: Yurii Paniv
        - Recording: https://youtu.be/9hHF91aZIOk
    4. Homework
        - Google Form: https://forms.gle/r6seb6MRH7a2d7GcA
        - Practical Task: Homework Section in https://github.com/VSydorskyy/ucu_audio_processing_course/blob/main/Module_3/Lecture_2/SpeakerDiarization.ipynb
        - Deadline: 14.04.2025, 24:00 GMT +02:00
4. [] ASR
    1. [x] Introduction to Generative Models.
        - Author: Andrii Shevtsov
        - Recording: https://youtu.be/5ZCKRZUpAa8
    2. [x] Introduction to ASR
        - Author: Oles
        - Colab: https://colab.research.google.com/drive/1iJvuurEQDaOkBba2zm1DSEkcdNDGhmU4
        - Recording:
    3. [x] Deeper ASR overview. CTC loss and Encoder architecture for ASR
        - Author: Yurii Laba
        - Recording:
    4. [x] Introduction into Transformers. Whisper
        - Author: Yurii Laba
        - Recording:
5. [] TTS
    1. [] TTS. Sequence-2-Sequence models
        - Author: Andrii Zhuravlov
        - Recording:
    2. [] TTS. Language Modelling approach
        - Author: Yevhenii
        - Recording:
6. [] Speech 2 Speech
    1. [] S2S. Diffusion model 
        - Author: Yevhenii and Volodymyr
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

## 2024

Raw table: https://docs.google.com/spreadsheets/d/1zpYV6K_BtvOUqX09dIwwgJLwhoPH0q5Eu7ZaOF0-fcA/edit?usp=sharing

# Citation

```
@misc{ucu_audio_processing_course_2024,
  author = {Volodymyr Sydorskyi, Anton Bazdyrev, Oles Dobosevych, Yurii Laba, Andrii Shevtsov, Taras Sereda},
  title = {UCU Audio Processing Course 2024},
  year = {2024},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/VSydorskyy/ucu_audio_processing_course}},
}
```
