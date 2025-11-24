# DSRP-B
A repository to archive the Data Science Research Project B -  Building a Data Pipeline for the collection,
preprocessing and analysis of Video-Music
Pairs.
This repository contains an end-to-end, reproducible pipeline for collecting, cleaning and enriching **Creative Commons BY–licensed video–music pairs** from YouTube.

The pipeline is organised into nine stages: (S0–S8), each implemented as a separate notebook/script. Together they transform raw CC BY videos into a **research-ready dataset** of short, standardised, semantically enriched video–music segments with:

- consistent video/audio formats  
- loudness-normalised audio  
- fixed-length segments  
- deduplicated clips  
- audio & visual embeddings  
- weak genre labels  
- BLIP-generated captions

The pipeline is implemented in Python and uses PyTorch, Hugging Face Transformers, librosa, ffmpeg, yt-dlp, and related tools.
Core scientific stack
	•	numpy (e.g. >=1.24)
	•	pandas (e.g. >=2.0)
	•	scipy (optional, for some signal ops)
	•	tqdm

Machine learning
	•	torch (e.g. >=2.1)
	•	torchvision (for CLIP image transforms)
	•	torchaudio (optional, some audio helpers)
	•	scikit-learn (e.g. >=1.3) – logistic regression, scaling, metrics

Audio processing
	•	librosa (e.g. >=0.10)
	•	soundfile (for WAV I/O)

System dependency:
	•	ffmpeg (must be installed on your system and on PATH)

Video download & handling
	•	yt-dlp (Python package or CLI; used in S0)
	•	python-dateutil / pytz (for timestamps, if used)

Vision & language models
	•	transformers (e.g. >=4.40) – for BLIP and CLIP, depending on your implementation
	•	huggingface_hub (optional but recommended)
	•	Pillow – image loading for BLIP/CLIP
  
Plotting / EDA 
	•	matplotlib
	•	seaborn
