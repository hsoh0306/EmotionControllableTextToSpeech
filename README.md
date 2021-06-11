# Emotion Controllable Text-to-Speech based on FastSpeech 2 

![](./assets/model.png)
# Introduction
Recently, speech synthesis research has developed rapidly, and many studies are now underway on Emotional Text-to-Speech (ETTS). However, there are many challenges with ETTS. Not only is it accompanied by considerable financial problems, but it is even more impossible to obtain the emotional strength label data. In this paper, we propose an unsupervised emotion labeling method and a controllable ETTS model to solve these problems. Emotion scores are given to emotion speech data using relative ranking functions, which are converted to emotion vectors and used as conditions in speech synthesis models. The emotion vector represents the emotion category and strength, which makes it easy to control emotional information. Experiments show that the proposed model controlled via emotion vectors can synthesize natural, emotion-expressive speech.

Implementation by PyTorch

Language: Korea

# Train
```
python train.py
```

# Synthesis
```
python synthesis.py --step 500000
```

# Train and synthesis results
## Pretrained model
### FastSpeech2 
[https://drive.google.com/file/d/1_YyQsmE4Dtxl-J5eXJnmcO4O7KKFLmmv/view?usp=sharing](https://drive.google.com/file/d/1_YyQsmE4Dtxl-J5eXJnmcO4O7KKFLmmv/view?usp=sharing)

### Hi-Fi GAN
[https://drive.google.com/file/d/1nqPDjqEr1oq0T7ezuZTfhBKMtHQgmHOL/view?usp=sharing](https://drive.google.com/file/d/1nqPDjqEr1oq0T7ezuZTfhBKMtHQgmHOL/view?usp=sharing)

## Training visualizing
![](./assets/tensorboard.png)
![](./assets/eval.gif)

## Melspectrogram, f0, energy
![](./assets/neu.png)



# References
- Y. Ren, *et al*., "[FastSpeech 2: Fast and High-Quality End-to-End Text to Speech](https://arxiv.org/abs/2006.04558)," *ICLR*, 2021
