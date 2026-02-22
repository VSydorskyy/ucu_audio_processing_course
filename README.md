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

1. [x] Into to Pytorch. Basic Deep Learning Tasks
    1. [x] Intro to Basic Pytroch. CNNs. Image Classification
        - Author: Volodymyr (Ostap)
        - Recording: https://youtu.be/D3kd1bzvOEM
        - Audience: UCU
        - Date: 19.01.2026
    2. [x] Intro to Lightning. RNNs. Named Entity Recognition
        - Author: Volodymyr (Volodymyr + Anton)
        - Recording: https://youtu.be/L98vDBEDNPQ
        - Audience: UCU
        - Date: 26.01.2026
    3. [x] Validation 
        - Author: Volodymyr (Anton)
        - Recording: https://youtu.be/_541B06AH-Y
        - Audience: UCU + KPI
        - Date: 02.02.2026
2. [x] Intro in Audio. Basic Audio Processing
    1. [x] Intro in Audio and Audio ML. Digital wave representation. Spectral audio representation
        - Author: Anton Ankudinov and Volodymyr
        - Recording: https://youtu.be/atCFO2y2jcU
        - Audience: UCU + KPI
        - Date: 09.02.2026
    2. [] Pre-processing, Filtering, Clustering
        - Author: Volodymyr (Oles)
        - Recording: 
        - Audience: UCU + KPI
        - Date: 16.02.2026
    3. [x] Self Supervised Audio Representations
        - Author: Yurii Yelisieiev 
        - Recording: 
        - Audience: UCU + KPI
        - Date: 23.02.2026
    4. Homework
        - Google Form: https://forms.gle/Fm1FskfWbr5cSXaH9 
        - Practical Task: Module_2/Аудіо МЛ. Лаброраторна №1.pdf
        - Deadline: 16.03.2026
3. [x] Audio Classification and Diarization
    1. [x] Audio Classification model
        - Author: Volodymyr
        - Recording: 
        - Audience: UCU + KPI
        - Date: 02.03.2026
    2. [] Speaker diarization 
        - Author: Yurii Paniv
        - Recording: 
        - Audience: UCU + KPI
        - Date: 09.03.2026
    3. Homework
        - Google Form: 
        - Practical Task:
        - Deadline: 
4. [x] ASR
    1. [x] Introduction to Generative Models.
        - Author: Andrii Shevtsov
        - Recording: 
        - Audience: UCU + KPI
        - Date: 16.03.2026
    2. [] Introduction to ASR
        - Author: Danil
        - Recording: 
        - Audience: UCU + KPI
        - Date: 23.03.2026
    3. [] Deeper ASR overview. CTC loss and Encoder architecture for ASR
        - Author: Yurii Laba
        - Recording: 
        - Audience: UCU + KPI
        - Date: 30.03.2026
    4. [] Introduction into Transformers. Whisper
        - Author: Danil
        - Recording: 
        - Audience: UCU + KPI
        - Date: 06.04.2026
    5. Homework
        - Google Form:
        - Practical Task:
        - Deadline: 
5. [x] TTS
    1. [x] TTS. Sequence-2-Sequence models
        - Author: Yevhenii
        - Recording: 
        - Audience: UCU + KPI
        - Date: 13.04.2026
    2. [x] TTS. Language Modelling approach
        - Author: Danil
        - Recording: 
        - Audience: UCU + KPI
        - Date: 20.04.2026
    3. [] TTS. Diffusion Approach
        - Author: Yevhenii
        - Recording: 
        - Audience: UCU + KPI
        - Date: 27.04.2026
    4. Homework
        - Google Form:
        - Practical Task: 
        - Deadline: 
6. [x] Project

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
@misc{ucu_audio_processing_course_2025,
  author = {Volodymyr Sydorskyi, Anton Bazdyrev, Oles Dobosevych, Yurii Laba, Andrii Shevtsov, Ostap Viniavskyi, Yurii Yelisieiev, Yurii Paniv, Andrii Zhuravlov, Yevhenii Azarov},
  title = {UCU Audio Processing Course 2025},
  year = {2025},
  publisher = {GitHub},
  journal = {GitHub repository},
  howpublished = {\url{https://github.com/VSydorskyy/ucu_audio_processing_course}},
}
```
