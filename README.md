# TorToiSe

Tortoise is a text-to-speech program built with the following priorities:

INSTALL GUIDE!

Python 3.9 - https://www.python.org/downloads/release/python-390/

Anaconda - https://www.anaconda.com/download

Git - https://gitforwindows.org/

go to start and run anaconda prompt

conda create --name tortoise-tts python=3.9

conda activate tortoise-tts

conda install -n base conda-forge::mamba

mamba install pandas

cd anaconda3

conda install torchaudio pytorch-cuda=11.7 -c pytorch -c nvidia
or if you have CPU and not Nvidia
pip3 install torch torchvision torchaudio

conda install -c conda-forge pysoundfile

git clone https://github.com/PlushBanshee/tortoise-tts.git

cd tortoise-tts

python -m pip install -r ./requirements.txt

conda install numba

python setup.py install

any time you want to use do
open conda and type

conda activate tortoise-tts
cd anaconda3
cd tortoise-tts

This script allows you to speak a single phrase with one or more voices.
python tortoise/do_tts.py --text "I'm going to speak this" --voice random --preset fast

This script provides tools for reading large amounts of text.
python tortoise/read.py --textfile <your text to be read> --voice random
