# DCNet:Weakly Supervised Saliency Guided Dual Coding Network for Visual Sentiment Recognition

## Introduction
Visual sentiment recognition is a challenging task with scientific significance in probing vision-processing mechanisms. Recent approaches mainly focused on using overall images or precise annotations to learn emotional representations, yet neglected to capture abstract semantics from regional information, or led to a heavy annotation burden. In this paper, we propose an end-to-end weakly supervised framework, called **Dual Coding Network** (DCNet), which models a dual coding process for both shallow features and high-level regional information. On the one hand, with the help of the fine-grained module (FG), visual features (e.g. texture features) are utilized to enhance the learning of distinguished representation. On the other hand, the DCNet innovatively leverages saliency information to imitate the neural decoding of perceived visual sentiment contents in human brain activity. Specifically, the saliency information guides the generation of sentiment-specific pseudo affective maps (SAMG), which serve as weak annotations. Then the DCNet couples fine-grained features with pseudo affective maps, and obtains semantic vectors for final sentiment prediction. Extensive experiments show that the proposed DCNet outperforms the state-of-the-art performance on five benchmark datasets. 

## Architecture
![](https://github.com/xyzhangw/DCNet/blob/main/framework.jpg)

## Dependencies
- <code>python</code> (tested on python3.7)
- <code>PyTorch</code>  (tested on 1.2.0)
- <code>torchvision</code>  (tested on 0.4.0)


## Data Preparation
 1. Download large-scale dataset FI-8 [here](https://drive.google.com/drive/folders/1gz5WhybpFT7F3YJ8Hl-6gxYWq12Gmbax?usp=drive_link), and put the splited dataset into <code>CausVSR/FI</code>.
 2. Download small-scale dataset [Emotion-6](http://chenlab.ece.cornell.edu/downloads.html).


## Train
1. Launch training by the command below:
   ```
   $ python main.py
   ```
  
## References
Our code is developed based on:
- [WSCNet: Weakly Supervised Coupled Networks for Visual Sentiment Classification and Detection.](https://ieeexplore.ieee.org/document/8825564)

Thanks for their great work!


## Citation
If you find our framework useful in your research, please consider citing:
```
@incollection{zhang2023dcnet,
  title={DCNet: Weakly Supervised Saliency Guided Dual Coding Network for Visual Sentiment Recognition},
  author={Zhang, Xinyue and Xiang, Jing and Zhang, Hanxiu and Wu, Chunwei and Wang, Hailing and Cao, Guitao},
  booktitle={ECAI 2023},
  pages={3050--3057},
  year={2023},
  publisher={IOS Press}
}
```
