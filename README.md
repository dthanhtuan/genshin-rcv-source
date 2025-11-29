### Install Python 3.11.12 and libs
```bash
curl https://pyenv.run | bash
pyenv install 3.11.12
pyenv virtualenv 3.11.12 .venv311
pyenv local .venv311
python --version
````
### Install torchvision torchaudio
```bash
pip install torch torchvision torchaudio pyworld
```

###  Install ffmpeg
[ffmpeg](https://ffmpeg.org/)

### Install fairseq
```bash
pip install fairseq_source/fairseq-0.12.3.1-cp311-cp311-linux_x86_64.whl
```

### Install Dependencies<br />
```bash
pip install -r requirements.txt
```

### Download Pre-model 
```bash
# Hubert Model
https://huggingface.co/lj1995/VoiceConversionWebUI/blob/main/hubert_base.pt
# Save it to /assets/hubert/hubert_base.pt

# RVMPE (rmvpe pitch extraction, Optional)
https://huggingface.co/lj1995/VoiceConversionWebUI/blob/main/rmvpe.pt
# Save it to /assets/rvmpe/rmvpe.pt
```

### Run WebUI <br />
```bash
python app.py
```