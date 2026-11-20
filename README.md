# Option C — Environmental sound analysis

**Mahir Foysol Chowdhury**

This experiment compares two spectrogram window lengths on the supplied dog clip `data/classification/1-100032-A-0.wav`. The original file is mono at 44.1 kHz and lasts 5 s. The clip derives from [rose_bark.wav by nfrae](https://freesound.org/people/nfrae/sounds/100032/) (CC0 per the course attribution). The course manifest identifies the ESC-50 package as CC BY-NC 3.0.

## Run the notebook

1. Keep the included `audio/` folder beside `analysis.ipynb`. It contains the single selected course recording.
2. In a Python environment, run `python -m pip install jupyterlab numpy scipy matplotlib ipython` and then `jupyter lab`.
3. Open `analysis.ipynb`, run all cells and save the notebook. The figures are written to `results/`.

## Settings and findings

I used 16 kHz mono audio, Hann windows of 512 and 2048 samples, and a fixed 160-sample hop (10 ms). The stronger activity occurs at about 2.20–2.50 s, with prominent components in the 0.8–1.8 kHz region. The 512-sample window localizes rapid changes more clearly. The 2048-sample window shows narrower frequency structure and spreads rapid changes across a longer time span.

The analysis uses one clip, so its timing and frequency peaks cannot be generalized to all dog barks.

## AI assistance

I used ChatGPT to adapt the lecture approach, execute the analysis, draft the interpretation and package the results.
